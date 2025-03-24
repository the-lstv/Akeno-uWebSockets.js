# Akeno uWebSockets.js
This is a fork of [uWebSockets.js](https://github.com/uNetworking/uWebSockets.js) which integrates [Akeno's](https://github.com/the-lstv/Akeno) router and caching among other features directly in C++ for lower latency and reduced callbacks to JS.

## See the [Akeno](https://github.com/the-lstv/Akeno) project
If you didnt mean to modify the core server of Akeno, you are probably looking for the original Akeno repository. [You can find it here.](https://github.com/the-lstv/Akeno)

## Buliding:
> [!WARNING]
> Akeno is currently only officially supported on Linux x86_64. Running on Windows or MacOS may not work as expected and we currently do not provide building instructions for it as it is not conclusive.

1. Clone the repository
```sh
git clone --depth=1 --recurse-submodules --shallow-submodules https://github.com/the-lstv/Akeno-uWebSockets.js
```
2. Compile the bulid.c file
```sh
gcc build.c -o build
```
3. Run the build file
```sh
./build
```
## Usage:
Copy the `dist` folder's content to your Akeno distribution folder to `/core/server/dist`, then fully restart the server with "akeno restart".


## License
Code under uWebSockets.js, uWebSockets and uSockets is intelectual property of [Alex Hultman](https://github.com/uNetworking) and is licensed under the Apache 2.0 License. Refer to the original repository and comments in source code for more information.

Modifications made by TheLSTV for Akeno are licensed under the GPL 3.0 License, the same as the Akeno project.
