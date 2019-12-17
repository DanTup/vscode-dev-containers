FROM debian:stretch

ENV PATH="$PATH":"/workspace/android/tools/bin":"/workspace/android/platform-tools":"/workspace/flutter/bin"
ENV ANDROID_SDK_ROOT="/workspace/android"

RUN apt-get update \
    && apt-get -y install git procps wget curl unzip lib32stdc++6

# Clean up
RUN apt-get autoremove -y \
    && apt-get clean -y \
    && rm -rf /var/lib/apt/lists/*

RUN mkdir /workspace
WORKDIR /workspace

RUN git clone --branch stable https://github.com/flutter/flutter \
    && flutter doctor
