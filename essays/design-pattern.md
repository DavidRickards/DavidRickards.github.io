---
layout: essay
type: essay
title: "Building And The Patterns Of Design"
# All dates must be YYYY-MM-DD format!
date: 2023-11-29
published: true
labels:
  - Personal Writing
  - Design Pattern
---

# The Makings Of A Great House 

Building a website is similar to building a house, but without all the manual labor. During the build process architects will have methods in which they will use to construct and when they run into commonly found problems they have a favorable protocol already ready to fix the situation. This protocol, these solutions are what can be referred to as a “[design pattern](https://sourcemaking.com/design_patterns).” To  be specific, a generic repeatable solution to a commonly occurring problem that not only ensures a sturdy structure but also aesthetically pleasing and adaptable.  

![image](https://damassets.autodesk.net/content/dam/autodesk/images/solutions/2d-cad-drafting-drawing/2d-drawing-thumb-1172x660-v1.jpg)

# The Big Three Blueprints

While many common problems and as such there exist a multitude of patterns but they can all be organized into three main blueprints, patterns. Creational design patterns are like blueprints that guide the creation of the house's foundation and framework. Think of structural design patterns as the blueprint for the architectural framework that defines how different components come together to form the large cohesive structure that becomes the functional house. In the dynamic life of a house, behavioral design patterns are blueprints that dictate how different elements interact and communicate within the house. Together, these design patterns ensure a well-architected digital structure, much like the combination of foundational plans, construction frameworks, and smart systems in building a resilient and functional house.

# Hidden Patterns Revealed

Before writing this essay I knew nothing about design patterns, despite this, I was still implementing some of these patterns. Just like any good builder I started with the foundation. Singleton pattern was the implantation of a global component signin that was responsible for user authentication and was necessary for them to access the recipes on our kitchen recipe site. With a basic foundation in, I will move to some of the frameworks. Many users have restrictive diets so we added on tags to help identify what recipes are within their restrictions. This is apparently a decorator pattern. Since our recipes now have tags we unknowingly implemented a strategy pattern through the use of search features. This search feature allowed users to search by inputting the recipe name or filtering by the tags. This leads to our communication lines working in the background. We added in a favorites system so that users didn’t have to go searching for the recipe every time. When started the recipe changes its state to a favorite state by the current user, which is a state pattern, and appears on their favorites page. As I continue to unfold our digital structure, there are undoubtedly more hidden patterns, awaiting identification and implementation, that I will learn and hope to use consciously for the future.
