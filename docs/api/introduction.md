---
sidebar_position: 1
slug: /api
---

# Introduction

## About the Filen API

The Filen API is used by our first-party clients, and it is publicly documented to enable external developers to build their own clients and other third-party applications on top of Filen.

The Filen API can do everything our first-party clients can, which includes uploading and downloading files, managing files and directories, sharing items, accessing notes and contacts, having chat conversations, managing user-specific settings, and more.

:::info SDKs

If you're building an application written in JavaScript or TypeScript, we recommend using our [TypeScript SDK](https://github.com/FilenCloudDienste/filen-sdk-ts), which provides developer-friendly wrappings of all API endpoints, and more.

There is also a [Go SDK](https://github.com/FilenCloudDienste/filen-sdk-go) that provides functionality for uploading/downloading and managing files and directories. It is currently work in progress!

If you need another reference for how to interface with the API or how to implement a specific process, the SDKs might be worth looking into.

:::

## How these docs are structured

In the following guides you will learn everything you need to know to access Filen in your own applications. The _Guides_ will walk you through authentication, how to properly encrypt and decrypt data, and how to upload and download files. Refer to the _Endpoints_ for detailed information about the available API endpoints, which includes more features such as sharing, notes, contacts, chats, and other.
