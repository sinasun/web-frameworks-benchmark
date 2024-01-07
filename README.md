# Web Frameworks Benchmark

Goal of this repository is to see if the already exist frontend and backend frameworks are optimized for production in term of speed.
With a focus on using WASM in frontend, and Server-side rendering using the backend frameworks to render fronend.

## Steps

### Server-side Rendering Benchmark

First step is by comparing all server side rendering engine for frontend, such as Next.js and Nest.js (which uses node.js as backend) with faster backend frameworks such as Golang.
We're trying to find the best option that can be used for server-side rendering, that is not being used right now.

### WASM in Frontend

Next step is by comparing computing tasks and features that frontend frameworks such as React/Vue/Angular/Elm/Svelte/Solid have to WASM (written in Rust, Golang and AssemblyScript).

We don't want to replace vanillajs/frameworks with WASM.
We need a list of case studies for when frameworks and vanillajs are not the ideal option.

By finding what features (such as hooks and DOM rendering to more complex features), frameworks are providing that is hard to implement in vanillajs, and having a benchmark on the features vs the same functionality written in WASM,
we can see what can WebAssembly replace.

## Frontend Frameworks Market Analysis

### Why Should People Choose a Framework

I believe the best understanding of how frontend people mind works is by looking at why everyone uses React:

- Popularity (More jobs)
- Easy to Learn
- A lot of Libraries
- Not complex for **most** of frontend apps (average frontend apps, are literally html/css with some API calls, and some states for updating page)
- TODO: to be added more

### Why Some Frameworks Faild

#### HTMX

It doesn't not support states and updating page, which most of apps are requiring this feature. Also I don't think this is the best way for large projects (same as Alpine.js).

#### Solid

Not popular enough which means very low amount of jobs and libraries for it.
It's super fast (way way better than React) and easy to learn (like React) but I believe the performance of it, is not enough to convince everyone to use it.

#### Angular

Hard to learn, not super fast in compare to other options. But still it's used due popularity and it's advantage for complex web apps.

#### Vue

Some technical issue that Vue doesn't support. But even if they fix them, still the popularity of React, which means more jobs and libraries beats Vue.

#### Alpine.js

Not complex enough for large projects.

#### Yew

It uses rust hype, but it's super hard to learn, and it's trying to replace javascript by itself.

TODO: To be added more

## Solutions

### Then How to Beat React?

Well it's hard. But a lot of dominant technologies such as PHP failed. So it's possible.
Specially because in most of the cases React is not having an actual advantage other than popularity.

There are a few ways until now I found that other frameworks could beat React, lets review them:

- Easier to code than React: Among of all other options for frontend, HTMX seems very easy and straight forward.
  But still we can see that htmx cannot fully replace React, specially when it comes to state handling, and scaling to more complex apps.

- Adding features to React: Same thing that Nextjs has done, by adding features such as server rendering, it becamse super popular.
  The advantage of this way, is that developers have lower learning curve than moving to other frameworks.
  Also, it supports most of libraries for React.

- Better Performance: Solid and Svelte has done it.

- New Technology: WebAssembly is a new technology in the market. It has the hype for now. Also Golang and Rust have their hypes for developers.

-

### Challenges

- Scaling: Having a framework that can be scale easily such as Vue and React is super hard. Angular is super bad for small projects, htmx/alpinejs is super bad for large projects.

- Jobs: One of the most important for new developers to learn a framework is how much jobs it has.

  - This can happen is years, by gradually moving to new frameworks.
  - Or by a hype, such as Rust hype which a super big (in compare to Golang and WebAssembly hype)
  - Or it can happen by not trying to replace a framework totally. So if someone learn your framework, learns React too.

- Libraries: React has a lot of libraries. Trying recreate all of them, means a huge waste of time.

  - By having a framework that supports React libraries, you can take the advantage of all React libraries.
    This is how TypeScript replaced JavaScript.

- All in One Solution: Having all of the solutions seems not possible and making the framework more complex.

### Ideas

- Gradually adding feature to a new framework to replace rather than coming up with a totally new framework.
