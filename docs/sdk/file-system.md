---
sidebar_position: 4
slug: /sdk/file-system
---

# File System

The SDK provides a virtual file system class which closely follows the "Node.js style of accessing the local file system". You can create files, read directories, delete items, create streams and much more.

:::tip Refer to generated SDK docs

If you need in depth information about implemented functions and types you can always take a look at the [generated SDK docs](https://sdk-ts-docs.filen.io/classes/_internal_.FS.html).

:::

### Examples

```ts
// Create a directory
await filen.fs().mkdir({
	path: "/Pictures"
})

// Upload a file
await filen.fs().upload({
	path: "/Pictures",
	source: "/Local/path/to/a/file.jpg"
})

// Read contents of the directory at path
const content: string[] = await filen.fs().readdir({
	path: "/Pictures"
})

// Stat a file
const stats: FSStats = await filen.fs().stat({
	path: "/Pictures/file.jpg"
})

// Download a file
await filen.fs().download({
	path: "/Pictures/file.jpg",
	destination: "/Local/path/to/a/file.jpg"
})

// Read a file
const content: Buffer = await filen.fs().readFile({
	path: "/Pictures/file.jpg"
})

// Write to a path
await filen.fs().writeFile({
	path: "/text.txt",
	content: Buffer.from("foobar", "utf-8")
})
```
