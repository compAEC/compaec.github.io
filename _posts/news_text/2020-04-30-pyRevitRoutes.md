---
layout: post
title:  "pyRevit Routes (HTTP API)"
date:   2020-04-30 16:39:30 +1000
categories: news
---

Control Revit from a web application

From [pyRevit-Routes-HTTP-API](https://www.notion.so/pyRevit-Routes-HTTP-API-79ef6d4a77b04aca9be6f4e46ffa728e)
Let's say we want to create a web application that would display a list of doors in a model. The web application would be split into two parts.

- **Font-end**: the part that runs in the browser and acts as the user interface, and
- **Back-end**: the part that the front-end contacts to send and receive data

While you are free to select whatever toolchain and GUI framework (React, Vue.js, etc) you are comfortable with for the front-end, the challenge has always been on how to create a back-end that has access to Revit contexts and can query or modify Revit documents. What we really needed is to run a HTTP web server over a running Revit instance and manage the HTTP calls in a way that would be executed in Revit context.

The new **Routes** python module, is an HTTP micro-framework to create web APIs running over Revit instances. This means that you can create functionality that could be triggerd from remote. This framework provides the necessary mechanism to create a back-end that has access to Revit context.

<iframe width="560" height="315" src="https://www.youtube.com/embed/rUCM0pJz5Zw" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Also worth looking at Radu Gidei's [DynaServer](https://github.com/radumg/DynaServer) implemented for Dynamo.