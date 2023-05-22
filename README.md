[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![License][license-shield]][license-url]

# Redis Recipe for Spring Boot with GeoSpatial Data Types

[![arm64-native](https://circleci.com/gh/dashaun/redis-recipes-spring-boot-geospatial.svg?style=shield)](https://app.circleci.com/pipelines/github/dashaun/redis-recipes-spring-boot-geospatial) |
[![amd64-native](https://github.com/dashaun/redis-recipes-spring-boot-geospatial/actions/workflows/amd64-native.yml/badge.svg)](https://github.com/dashaun/redis-recipes-spring-boot-geospatial/actions/workflows/amd64-native.yml)


## | [Prerequisites](#prerequisites) | [Quick Start](#quick-start) | [Build Native Image](#build-native-image) | [Native Image Test](#native-image-test) | [See Also](#see-also) | [Contributing](#contributing) | [License](#license) |

## Prerequisites

- Java 17 or above
- [GraalVM](https://graalvm.org) 22.3 or above

## Quick Start

```bash
git clone https://github.com/dashaun/redis-recipes-spring-boot-geospatial
cd redis-recipes-spring-boot-geospatial
./mvnw spring-boot:run
```

## Build Native Image

```bash
./mvnw -Pnative spring-boot:build-image
```

## Multi-architecture buildpack

This repository uses [dashaun/builder:tiny](https://hub.docker.com/r/dashaun/builder)
which allows you to create `native` images for both AMD64 and ARM64 architectures.
I'm trying to take the `ARM64` support upstream to [Paketo](https://paketo.io), so any feedback you have from using this buildpack, with this project or any other is greatly appreciated!

## See Also

- [Spring Cloud Gateway 4.0.0-rc2 native example with Testcontainers](https://dashaun.com/posts/spring-cloud-gateway-4-0-0-rc2-native-example-with-testcontainers/)
- [Cloud Native Buildpack for ARM64 and AMD64](https://dashaun.com/posts/java-native-builder-multiarch-7-41-0/)
- [First attempt at a multi-architecture buildpack](https://dashaun.com/posts/multiarch-builder-poc/)
- [K3s Knative Ubuntu Raspberry Pi](https://dashaun.com/posts/k3s-knative-ubuntu-raspberry-pi/)

<!-- CONTRIBUTING -->
## Contributing

### Release

- git tag v#.#.#
- git push origin v#.#.#

Pull-requests are welcomed!

<!-- LICENSE -->
## License

Distributed under the Apache License, Version 2.0. See `LICENSE` for more information.

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/dashaun/redis-recipes-spring-boot-geospatial.svg?style=for-the-badge
[contributors-url]: https://github.com/dashaun/redis-recipes-spring-boot-geospatial/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/dashaun/redis-recipes-spring-boot-geospatial.svg?style=for-the-badge
[forks-url]: https://github.com/dashaun/redis-recipes-spring-boot-geospatial/network/members
[stars-shield]: https://img.shields.io/github/stars/dashaun/redis-recipes-spring-boot-geospatial.svg?style=for-the-badge
[stars-url]: https://github.com/dashaun/redis-recipes-spring-boot-geospatial/stargazers
[issues-shield]: https://img.shields.io/github/issues/dashaun/redis-recipes-spring-boot-geospatial.svg?style=for-the-badge
[issues-url]: https://github.com/dashaun/redis-recipes-spring-boot-geospatial/issues
[license-shield]: https://img.shields.io/github/license/dashaun/redis-recipes-spring-boot-geospatial.svg?style=for-the-badge
[license-url]: https://github.com/dashaun/redis-recipes-spring-boot-geospatial/blob/master/LICENSE.txt
