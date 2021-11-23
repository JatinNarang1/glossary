---
title: Stateful Apps
status: Feedback Appreciated
category: concept
---

## What it is

Stateful (and [stateless](https://glossary.cncf.io/stateless_apps/))application, is a program that keeps track of the state of interaction with user and saves data(either locally or in database systems) for use in the next session. For example, while using an e-commerce website your cart information is stored and can also be accessed in the next session.

## Problem it addresses

Using an app generally requires multiple requests. For example, when online banking, you'll authenticate yourself by entering your password (request #1), then you may transfer money to a friend (request #2), and finally, you'll want to view transfer details (request #3). To function correctly, each step has to remember the previous ones, and the bank needs to remember the state of everyone’s accounts. Today, most applications we use are at least partly stateful, as they store things like preferences and settings to improve the user experience.

## How it helps

There are several ways to store state for a stateful application. The simplest is to hold the state in memory and not persist it anywhere. The problem with that is, whenever the application has to be restarted, all state is lost. In order to prevent that, state is persisted either locally (on disk) or in database systems. 
