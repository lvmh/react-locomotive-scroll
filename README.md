<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/toinelin/react-locomotive-scroll">
    <img src="https://user-images.githubusercontent.com/4596862/58807621-67aeec00-85e6-11e9-8e3a-3fe4123ee76c.png" alt="Logo" width="80" height="80">
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/a7/React-icon.svg/1200px-React-icon.svg.png" alt="Logo" height="60">
  </a>

  <h3 align="center">React Locomotive Scroll</h3>

  <p align="center">
    A locomotive-scroll React wrapper
    <br />
    <a href="https://github.com/locomotivemtl/locomotive-scroll"><strong>Explore Locomotive Scroll docs »</strong></a>
    <br />
    <br />
    <!-- <a href="https://github.com/toinelin/react-locomotive-scroll">View Demo</a>
    · -->
    <a href="https://github.com/toinelin/react-locomotive-scroll/issues">Report Bug</a>
    ·
    <a href="https://github.com/toinelin/react-locomotive-scroll/issues">Request Feature</a>
  </p>
</p>



<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary><h2 style="display: inline-block">Table of Contents</h2></summary>
  <ol>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgements">Acknowledgements</a></li>
  </ol>
</details>

## Getting Started

To get a local copy up and running follow these simple steps.

### Installation

```sh
$ npm install locomotive-scroll react-locomotive-scroll
```

or using [Yarn](https://yarnpkg.com/)

```sh
$ yarn add locomotive-scroll react-locomotive-scroll
```



<!-- USAGE EXAMPLES -->
## Usage

Import the provider
```js
import { LocomotiveScrollProvider } from 'react-locomotive-scroll'
```

Wrap your application using the provider
```js
const containerRef = useRef(null)

<LocomotiveScrollProvider
  options={
    {
      smooth: true,
      // ... all available Locomotive Scroll instance options 
    }
  }
  watch={
    [
      //...all the dependencies you want to watch to update the scroll
    ]
  }
  containerRef={containerRef}
>
  <main data-scroll-container ref={containerRef}>
    {/* ...your app */}
  </main>
</LocomotiveScrollProvider>
```

Wrap your pages using `data-scroll-section` to prevent weird behaviours

```js
export function Page() {
  return (
    <div data-scroll-section>
      {/* ...your page */}
    </div>
  )
}
```

Get the scroll instance through all your components
```js
import { useLocomotiveScroll } from 'react-locomotive-scroll'

export function Component() {
  const { scroll } = useLocomotiveScroll()

  // ... your component
}
```

At this time you should be able to do whatever your want using the scroll object.

For more examples and to use Locomotive Scroll, please refer to their [Documentation](https://github.com/locomotivemtl/locomotive-scroll)

<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` for more information.



<!-- CONTACT -->
## Contact

Antoine Lin - [@vahilloff](https://twitter.com/vahilloff) - contact@antoinelin.com

Project Link: [https://github.com/toinelin/react-locomotive-scroll](https://github.com/toinelin/react-locomotive-scroll)



<!-- ACKNOWLEDGEMENTS -->
## Acknowledgements

* []()
* []()
* []()

_Please feel free to open a pull request to add your project to the list!_




<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/toinelin/repo.svg?style=for-the-badge
[contributors-url]: https://github.com/toinelin/repo/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/toinelin/repo.svg?style=for-the-badge
[forks-url]: https://github.com/toinelin/repo/network/members
[stars-shield]: https://img.shields.io/github/stars/toinelin/repo.svg?style=for-the-badge
[stars-url]: https://github.com/toinelin/repo/stargazers
[issues-shield]: https://img.shields.io/github/issues/toinelin/repo.svg?style=for-the-badge
[issues-url]: https://github.com/toinelin/repo/issues
[license-shield]: https://img.shields.io/github/license/toinelin/repo.svg?style=for-the-badge
[license-url]: https://github.com/toinelin/repo/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/toinelin