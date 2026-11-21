FROM ruby:3.4-bookworm

# 빌드 및 Git 관련 패키지
RUN apt-get update && apt-get install -y --no-install-recommends \
    build-essential \
    git \
    && rm -rf /var/lib/apt/lists/*

# Bundler 의존성 설치 위치
ENV BUNDLE_PATH=/usr/local/bundle
ENV PATH="${BUNDLE_PATH}/bin:${PATH}"

WORKDIR /workspace
