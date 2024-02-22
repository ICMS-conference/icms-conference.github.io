---
layout: session
title: "ICMS 2024 - Session 13: General Session"
---
### Organizers
   * [Yue Ren](https://yueren.de)<br/>

### Aim and Scope
This session addresses aspects of mathematical software that not covered by the other sessions.

## Accepted Talks

#### Integrating GeoGebra with React and WebAssembly: A Web-Based Approach for Mathematical Software Development
#### [Mitsushi Fujimoto](mailto:fujimoto@fukuoka-edu.ac.jp) (University of Teacher Education Fukuoka, Japan)


A dynamic mathematics software GeoGebra can be embedded on the web, and a
JavaScript API is provided for interaction. By utilizing web platforms, GeoGebra
can collaborate with various web technologies. In this talk, I would like to
introduce a method for creating a GeoGebra-based web app using React for the UI
and WebAssembly for the computational engine.

React is a JavaScript library for creating rich UI components and writing clean
code using JSX. It can detect code errors during the transpilation of JSX to
regular JavaScript. The use of React can address the limitations of GeoGebra's
script input dialog. WebAssembly (Wasm) is a binary format that can run C
functions in web browsers. The web app version of GeoGebra can access external
computational engines created in C language using WebAssembly.

The implementation process includes creating a React component for GeoGebra
using react-geogebra, developing a computational engine in C, converting it to a
Wasm binary with Emscripten, and executing C functions from the React side to
update the UI dynamically.

Some considerations are required for the collaboration between React and
WebAssembly. I will explain the details through the implementation of a
mathematical puzzle, 'Lights Out'. The source code consists of 200 lines of
React code and 100 lines of C code. The web app can be accessed at
https://mitsushi-fujimoto.github.io/geo-lights/


#### The use of HTML-based dynamic content for the learning of statistical test
#### [Masataka Kaneko](mailto:masataka.kaneko@phar.toho-u.ac.jp) (Toho University, Japan)
#### [Takuya Kitamoto](mailto:kitamoto@yamaguchi-u.ac.jp) (Yamaguchi University, Japan)
#### [Takeo Noda](mailto:noda@c.sci.toho-u.ac.jp) (Toho University, Japan)

With the wide-spread availability of high-speed internet,
an HTML-based system is one of the most promising options
for mathematical software in this post COVID-19 era.
While many web-based software libraries are available
for specific purposes, including ones for symbolic calculations
and dynamic visualizations, extra elaboration is needed
to integrate their capabilities so that users can perform
mathematical activities on a single HTML content.

Moreover, it seems that the realities and benefits derived from
the use of those systems have not yet been fully investigated.
Especially in the complex case of statistics learning, more precise
knowledge about them will likely help maximize the effect of
using newly developed systems. This research is mainly concerned
with the use of our newly developed system for the learning
of the $\chi^2$ test for independence.
Through the comparative study of the log of simulations,
which learners performed on the HTML content between
experimental and control groups, it has been shown that
some restrictions to the context of its use can have
a large influence on learners' thinking.

Key Words:
HTML5, CindyJS, dynamic visualization, Jspreadsheet, Apache ECharts, Numerical Recipes
