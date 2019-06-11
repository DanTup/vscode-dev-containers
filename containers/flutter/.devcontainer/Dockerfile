FROM debian:stretch

ENV PATH="$PATH":"/workspace/android/tools/bin":"/workspace/android/platform-tools":"/workspace/flutter/bin"
ENV ANDROID_SDK_ROOT="/workspace/android"

RUN apt-get update \
    && apt-get -y install git procps wget curl unzip lib32stdc++6 openjdk-8-jdk

# Clean up
RUN apt-get autoremove -y \
    && apt-get clean -y \
    && rm -rf /var/lib/apt/lists/*

RUN mkdir /workspace
WORKDIR /workspace

RUN git clone --branch stable https://github.com/flutter/flutter \
    && flutter doctor

RUN wget https://dl.google.com/android/repository/sdk-tools-linux-4333796.zip \
    && unzip -d /workspace/android ./sdk-tools-linux-4333796.zip

RUN (yes | sdkmanager tools platform-tools) \
    && (yes | sdkmanager "platforms;android-28" "build-tools;28.0.3" "extras;google;m2repository" "extras;android;m2repository") \
    && (yes | flutter doctor --android-licenses)
