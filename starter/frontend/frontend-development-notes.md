# Frontend Development Notes

## React & TypeScript

The frontend of our Movie Picture application is written in TypeScript and uses the React framework. This means that the codebase adheres to strict type checking and a component-based structure. 

## eslint

This project uses eslint for code quality. It's important that all code adheres to the rules outlined in our `.eslintrc` file. The linter will automatically check your code for style issues, potential bugs, and enforce certain design principles. 

## React Testing Library

Our application uses the React Testing Library for unit testing. This testing library is focused on the user's perspective. The tests are designed to resemble how users interact with your app.

## GitHub Actions

GitHub Actions are used to automate our software development workflows. GitHub Actions will be responsible for running our linter, tests, and building the app whenever there is a `pull_request` against the `main` branch. It will also handle the deployment of our app whenever there is a `push` to the `main` branch. 

## Docker

We're using Docker to containerize our frontend application.

## Kubernetes

Deployment of our app to the existing Kubernetes cluster will be automated by our GitHub Actions workflows. 

## AWS & Terraform

We're using AWS to host our Kubernetes cluster and Terraform to manage our infrastructure as code. You'll need to create AWS infrastructure using the Terraform scripts provided. Follow the instructions in the exercise carefully and ensure you have the necessary permissions to perform these actions. 

---

As you work on this project, remember to focus on understanding each part of the pipeline. Make sure that all your workflows are correctly configured and that they trigger as expected. Keep the best practices in mind as you work and ensure that your code is clean and well-tested.
DEPRECATED: The legacy builder is deprecated and will be removed in a future relea
se.                                                                                           Install the buildx component to build images with BuildKit:
            https://docs.docker.com/go/buildx/

Sending build context to Docker daemon  292.1MB
Step 1/10 : FROM  public.ecr.aws/docker/library/node:18.14.2-alpine3.17
18.14.2-alpine3.17: Pulling from docker/library/node
63b65145d645: Pull complete 
061765f30124: Pull complete 
478140d59116: Pull complete 
00ca3aba45c3: Pull complete 
Digest: sha256:f8a51c36b0be7434bbf867d4a08decf0100e656203d893b9b0f8b1fe9e40daea
Status: Downloaded newer image for public.ecr.aws/docker/library/node:18.14.2-alpi
ne3.17                                                                             ---> 9423415aa47a
Step 2/10 : ARG REACT_APP_MOVIE_API_URL
 ---> Running in ee27f0e67618
 ---> Removed intermediate container ee27f0e67618
 ---> 1fda294a54d9
Step 3/10 : ENV REACT_APP_MOVIE_API_URL=${REACT_APP_MOVIE_API_URL}
 ---> Running in 4214ac3a4b08
 ---> Removed intermediate container 4214ac3a4b08
 ---> e9da192f2d3d
Step 4/10 : WORKDIR /app
 ---> Running in 74a357df62e1
 ---> Removed intermediate container 74a357df62e1
 ---> 3c3f2b60a3ef
Step 5/10 : COPY package*.json ./
 ---> c834a73f2a7f
Step 6/10 : RUN npm ci
 ---> Running in f48c20d3fddc
npm WARN deprecated w3c-hr-time@1.0.2: Use your platform's native performance.now(
) and performance.timeOrigin.                                                     npm WARN deprecated stable@0.1.8: Modern JS already guarantees Array#sort() is a s
table sort, so this library is deprecated. See the compatibility table on MDN: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/sort#browser_compatibility                                                      npm WARN deprecated rollup-plugin-terser@7.0.2: This package has been deprecated a
nd is no longer maintained. Please use @rollup/plugin-terser                      npm WARN deprecated sourcemap-codec@1.4.8: Please use @jridgewell/sourcemap-codec 
instead                                                                           npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN deprecated svgo@1.3.2: This SVGO version is no longer supported. Upgrade 
to v2.x.x.                                                                        npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown
npm WARN tar TAR_ENTRY_ERROR EINVAL: invalid argument, fchown

added 1506 packages, and audited 1507 packages in 30s

263 packages are looking for funding
  run `npm fund` for details

104 vulnerabilities (14 low, 48 moderate, 36 high, 6 critical)

To address issues that do not require attention, run:
  npm audit fix

To address all issues (including breaking changes), run:
  npm audit fix --force

Run `npm audit` for details.
npm notice 
npm notice New major version of npm available! 9.5.0 -> 12.2.0
npm notice Changelog: <https://github.com/npm/cli/releases/tag/v12.2.0>
npm notice Run `npm install -g npm@12.2.0` to update!
npm notice 
 ---> Removed intermediate container f48c20d3fddc
 ---> ac528ba83e01
Step 7/10 : COPY . .
 ---> fd2d1e6a04fd
Step 8/10 : RUN npm run build
 ---> Running in fbad0846c640

> frontend@1.0.0 build
> react-scripts build

Creating an optimized production build...
Browserslist: caniuse-lite is outdated. Please run:
  npx update-browserslist-db@latest
  Why you should do it regularly: https://github.com/browserslist/update-db#readme
Browserslist: caniuse-lite is outdated. Please run:
  npx update-browserslist-db@latest
  Why you should do it regularly: https://github.com/browserslist/update-db#readme
Compiled successfully.

File sizes after gzip:

  57.11 kB  build/static/js/main.2914319b.js
  556 B     build/static/css/main.86fcb180.css

The project was built assuming it is hosted at /.
You can control this with the homepage field in your package.json.

The build folder is ready to be deployed.
You may serve it with a static server:

  npm install -g serve
  serve -s build

Find out more about deployment here:

  https://cra.link/deployment

 ---> Removed intermediate container fbad0846c640
 ---> 24a9a69785a2
Step 9/10 : EXPOSE 3000
 ---> Running in 5b52646aa379
 ---> Removed intermediate container 5b52646aa379
 ---> 52121b9be6ea
Step 10/10 : CMD ["npm", "run", "serve"]
 ---> Running in f57db3f5faf6
 ---> Removed intermediate container f57db3f5faf6
 ---> 636e7d4fc50f
Successfully built 636e7d4fc50f
