---
uid: Tutorial.Composition
title: Composition
---

# Composition

Composition is a general term describing creation and initialization of an object. During composition an object is created and initialized with all of its dependencies and initialization methods.

Since each dependency might have its own dependencies entire dependency graph has to be created and each node has to be initialized in order of priority.

The Unity container supports two types of composition:

## Resolution

Resolution is a process where an object is built from scratch. In other words, the container is allocating the memory for an abject, calls a constructor with all of its dependencies and performs all necessary initialization required by the type. For more information see <xref:Tutorial.Resolution>

## Building Up

Building up is a process where the container does not create an object but initializes already created object. This is useful when an object is part of an infrastructure and author does not have access or control of how these are created.