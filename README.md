## npdVNC Web Front-End

<a href="https://npdweb.com"><img src="https://npd-static-content.s3.amazonaws.com/logo_npd.png" width="300"><a/>

npdVNC provides remote web-based access to a Desktop or application. While VNC is in the name, npdVNC differs from other VNC variants such as TigerVNC, RealVNC, and TurboVNC. npdVNC has broken from the RFB specification which defines VNC, in order to support modern technologies and increase security. npdVNC is accessed by users from any modern browser and does not support legacy VNC viewer applications. npdVNC uses a modern YAML based configuration at the server and user level, allowing for ease of management.

[npd Technologies](https://www.npdweb.com) developed npd Workspaces, the Containerized Streaming Platform. npd has open-sourced the Workspace docker images, which include containerized [full desktops and apps](https://github.com/npdtech/workspaces-images) and [base images](https://github.com/npdtech/workspaces-core-images) intended for developers to create custimized streaming containers. These containers can be used standalone or within the [npd Workspaces Platform](https://www.npdweb.com) which provides a full Enterprise feature set.

## News/Help/Contact

For support with npdVNC, post on the [npdVNC Project](https://github.com/npdtech/npdVNC).

## Documentation

**Do not use the README from the master branch**, unless you are compiling npdVNC yourself from the tip of master. Use the documentation for your specific release.

  - [npdVNC 1.0.0 Documentation](https://www.npdweb.com/npdvnc/docs/1.0.0/index.html)

  For beta releases prior to version 1.0.0, use the README in this github project on the tagged commit for that release.

## Features

  - Webp image compression for better bandwidth usage
  - Automatic mixing of webp and jpeg based on CPU availability on server
  - WebRTC UDP Transit
  - Lossless QOI Image format for Local LAN
  - [Dynamic jpeg/webp image coompression](https://github.com/npdtech/npdVNC/wiki/Video-Rendering-Options#dynamic-image-quality) quality settings based on screen change rates
  - Seemless clipboard support (on Chromium based browsers)
  - Binary clipboard support for text, images, and formatted text (on Chromium based browsers)
  - Allow client to set/change most configuration settings
  - Multi-User support with permissions that can be changed via the API
  - Web UI uses a webpack for faster load times.
  - Network and CPU bottleneck statistics
  - Relative cursor support (game pointer mode)
  - Cursor lock
  - IME support for languages with extended characters
  - Better mobile support

## Screenshots

<img src="https://5856039.fs1.hubspotusercontent-na1.net/hubfs/5856039/npdVNC_Screenshot_Features.png" width=600>


## Browser Requirements

For a full listing of features and minimum browser version required for each browser, see this [npdVNC Wiki Article](https://github.com/npdtech/npdVNC/wiki/Browser-Support).


## Server Requirements

npdVNC is an absolute requirement. This fork of noVNC is explicitly modified to work with npdVNC and breaks the RFB specification. It will not work with legacy VNC servers.

## Running noVNC

npdVNC has a built in web server and the web code is baked into npdVNC. There are no instructions to provide, just install npdVNC follow the instructions to configure and run it.

## Development

The noVNC code is webpacked for performance reasons. The CI pipeline in the npdVNC project is responsible for building the web code and packaging it with npdVNC.
