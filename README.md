## CICD DevSecOps Project   
<!--
[![Image](https://github.com/chaudharysurya14/CICD_Portfolio_maven_project/blob/master/webapp/src/main/webapp/img/project_workflow.png "DevOps Project - CI/CD with Jenkins Ansible Docker Kubernetes ")](https://www.udemy.com/course/valaxy-devops/?referralCode=8147A5CF4C8C7D9E253F) -->
<div align="center">
  <a href="http://netflix-clone-with-tmdb-using-react-mui.vercel.app/">
    <img src="https://github.com/chaudharysurya14/CICD_Portfolio_maven_project/blob/master/webapp/src/main/webapp/img/project_workflow.png" alt="Logo" width="100" height="32">
  </a>

  <h3 align="center">Portfolio_CICD_Project</h3>

  <p align="center">
    <a href="https://chaudharysurya14.github.io/cyber.playboy/">View Demo</a>
    ·
    <a href="saigalsainy318333@gmail.com">Report Bug</a>
    ·
    <a href="https://chaudharysurya14.github.io/cyber.playboy/">Request Feature</a>
  </p>
</div>

<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#prerequests">Prerequests</a>
    </li>
    <li>
      <a href="#which-features-this-project-deals-with">Which features this project deals with</a>
    </li>
    <li><a href="#third-party-libraries-used-except-for-react-and-rtk">Third Party libraries used except for React and RTK</a></li>
    <li>
      <a href="#contact">Contact</a>
    </li>
  </ol>
</details>

<br />

<div align="center">
  <img src="./public/assets/home-page.png" alt="Logo" width="100%" height="100%">
  <p align="center">Home Page</p>
  <img src="./public/assets/mini-portal.png" alt="Logo" width="100%" height="100%">
  <p align="center">Mini Portal</p>
  <img src="./public/assets/detail-modal.png" alt="Logo" width="100%" height="100%">
  <p align="center">Detail Modal</p>
  <img src="./public/assets/grid-genre.png" alt="Logo" width="100%" height="100%">
  <p align="center">Grid Genre Page</p>
  <img src="./public/assets/watch.png" alt="Logo" width="100%" height="100%">
  <p align="center">Watch Page with customer contol bar</p>
</div>

## Prerequests

- Install and setup svn server locally [SVNserver](https://subversion.apache.org/) for create a central repo
- Install jenkins and setup enviroment [Jenkins](https://www.jenkins.io/doc/book/installing/linux/). for automate all this project
- Install sonarqube and set enviroment [SonarQube](https://docs.sonarsource.com/sonarqube/latest/setup-and-upgrade/install-the-server/introduction/) for scan the source code.
- Install and configure [Nexus](https://www.fosstechnix.com/how-to-install-nexus-repository-on-ubuntu/) for store the artifacts.
- Install and configure [Tomcat](https://tomcat.apache.org/download-90.cgi) for deploy our application. 

## Which features this project deal with

- How to create and use [Custom Hooks](https://reactjs.org/docs/hooks-custom.html)
- How to use [Context](https://reactjs.org/docs/context.html) and its provider
- How to use lazy and Suspense for [Code-Splitting](https://reactjs.org/docs/code-splitting.html)
- How to use a new [lazy](https://reactrouter.com/en/main/route/lazy) feature of react-router to reduce bundle size.
- How to use data [loader](https://reactrouter.com/en/main/route/loader) of react-router, and how to use redux dispatch in the loader to fetch data before rendering component.
- How to use [Portal](https://reactjs.org/docs/portals.html)
- How to use [Fowarding Refs](https://reactjs.org/docs/forwarding-refs.html) to make components reusuable
- How to create and use [HOC](https://reactjs.org/docs/higher-order-components.html)
- How to customize default theme of [MUI](https://mui.com/)
- How to use [RTK](https://redux-toolkit.js.org/introduction/getting-started)
- How to use [RTK Query](https://redux-toolkit.js.org/rtk-query/overview)
- How to customize default classname of [MUI](https://mui.com/material-ui/experimental-api/classname-generator)
- Infinite Scrolling(using [Intersection Observer API](https://developer.mozilla.org/en-US/docs/Web/API/Intersection_Observer_API))
- How to make awesome carousel using [slick-carousel](https://react-slick.neostack.com)

## Third Party libraries used except for React and RTK

- [react-router-dom@v6.9](https://reactrouter.com/en/main)
- [MUI(Material UI)](https://mui.com/)
- [framer-motion](https://www.framer.com/docs/)
- [video.js](https://videojs.com)
- [react-slick](https://react-slick.neostack.com/)

## Install with Docker

```sh
docker build --build-arg TMDB_V3_API_KEY=your_api_key_here -t surya0010/cicdportfolio:41 .

docker run --name netflix-clone-website --rm -d -p 80:80 surya0010/cicdportfolio:41
```

## Todo

- Make the animation of video card portal more similar to Netflix.
- Improve performance. I am using `context` and `provider` but all components subscribed to the context's value are re-rendered. These re-renders happen even if the part of the value is not used in render of the component. there are [several ways](https://blog.axlight.com/posts/4-options-to-prevent-extra-rerenders-with-react-context/) to prevent the re-renders from these behaviours. In addition to them, there may be several performance issues.
- Replace bundler([Vite](https://vitejs.dev/guide)) with [Turbopack](https://turbo.build/pack/docs/why-turbopack). Turbopack is introduced in Next.js conf recently. It's very fast but it's nor ready to use right now. it just support Next.js, and they plan to support all others as soon as possible. so if it's ready to use, replace [Vite](https://vitejs.dev/guide) with [Turbopack](https://turbo.build/pack/docs/why-turbopack).
- Add accessibilities for better UX.
- Add Tests.
