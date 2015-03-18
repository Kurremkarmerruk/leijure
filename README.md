# Leijure

[![Join the chat at https://gitter.im/Kurremkarmerruk/leijure](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/Kurremkarmerruk/leijure?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

From antiquarian to clojurian. A walkthrough of Clojure and ClojureScript like no other.  This guide will bring you through a full-stack, single-page, web-app. What-fun!

## Attention

Several opinions reside here.  I like to think of myself as relatively discerning, but I strongly lack the real-world experience. I am really just doing this because teaching is my preferred way of learning things.  Whether this guide will be useful or come to completion is mostly unimportant as I'm in it for the process.  As I recently read, this is (in a way) my antiwork.  Doing something *I* want to do, the way *I* want to do it.

## Opinions

This is going to be a full-stack walkthrough.  I'll try to go over every decision I make with regards to server, tooling, editors, devops, and anything else that comes up!   I want the SPA to be fast, written entirely in clojure, and a nice blend of fun programmer-oriented features and user-facing enjoyment (compatibility, smoothness, gui speed, real-time updates).

## Current proposed stack:

- Tools:
  - [Leiningen](leiningen.org): Project management and build/automation toolset
  - [Light Table](http://lighttable.com/): Code editor with inline clojure repl.  Written entirely in ClojureScript!
  - [Figwheel](github.com/bhauman/lein-figwheel): A livereload plguin for leiningen with a browser repl
  - [Speclj](github.com/slagyr/speclj): A TDD/BDD framework for Clojure and ClojureScript. (If necessary)

- Server:
  - [Immutant 2](immutant.org): Immutant 2's web library is an abstraction over [Undertow](undertow.io), a java server
  - [Compojure](github.com/weavejester/compojure): A routing library (If necessary)
  - [Monger](clojuremongodb.info): Monger is an idiomatic Clojure abstraction over Java MongoDB driver

- Client:
  - [Clojurescript](github.com/clojure/clojurescript): A JS compiler leveraging Google's [Closure Compiler](developers.google.com/closure/compiler/)
  - [Reagent](reagent-project.github.io/): A ClojureScript interface to the [React](facebook.github.io/react/) library
  - [re-frame](github.com/Day8/re-frame): A framework/model built/designed around ClojureScript, Reagent, and   [FRP](https://gist.github.com/staltz/868e7e9bc2a7b8c1f754)
