# RSC Parser

This is a parser for React Server Components (RSC) when sent over the network. React uses a format to represent a tree of components/html or metadata such as requiered imports, suspense boundaries, and css/fonts that needs to be loaded.

I made this tool to more easily let you understand the data and explore it visually.

## Comparsion

<div style="display: flex; flex-direction: row;">

<img width="49%" alt="image" src="https://github.com/alvarlagerlof/rsc-parser/assets/14835120/f4384956-74e0-4647-a27e-b154a8716afa">

<img width="49%" alt="image" src="https://github.com/alvarlagerlof/rsc-parser/assets/14835120/f8f96e38-fc29-4348-8d83-1a04cd6322aa">
</div>



## How do I use this?

### Extension

I am currently developing a Chrome extension (Firefox hopefully soon) extension. Build artifacts are available [here](https://github.com/alvarlagerlof/rsc-parser/actions?query=branch%3Amain).

### Website

There is also a website that you can use by manually copy pasing RSC payloads.

1. Go to a site that uses the NextJS App router or generally is based on React Server components.
2. Open the network tab in your dev tools
3. Reload.
4. Look for fetch responses the payload roughly looks like json, but each like starts with something like `O:`, `1:I`, `b:` or similar.
5. Copy the text and paste it into the form on https://rsc-parser.vercel.app/
6. Explore!


## It crashed!
Please make an issue on https://github.com/alvarlagerlof/rsc-parser/issues/new and include the text content that the parser was unable to handle.

