---
layout: post
title:  "Backbone-DocumentModel"
date:   2015-05-30 13:50:51
categories: js, backbone  	
---


I've been working on a single page web appliction using [Backbone JS][backbonejs] and [Marionette][marionette] recently.
When working on one of the sections I wanted to create a parent-child view hierarchy:  a parent LayoutView which has a 
CompositeView child, as well as a CollectionView which itself has children CollectionViews.

Implementing this, I discovered something weird about Backbone models and collections: you can't have deeply nested 
model/collection structures by default; it's not possible to have a Backbone model which has Backbone models
as properties of it.

There is a few Backbone plugins which address this issue. The one I chose was [Backbone-DocumentModel][documentmodel].
This plugin even allows you to specify custom types as children of a particular model; so you can extend Backbone.Model
and have that type as a property of another Backbone.Model implementation.

It looks like the [Backbone-DocumentModel][documentmodel] project on Github might have been abandoned.  You'll notice if you try
install it through Bower, the latest version available is 0.6.0 although the version you'll actually want is 0.6.4.  This is
because the owner of the repo has not created a release for 0.6.4.  As a work-around, [I forked their repo][myrepo],
created a version for 0.6.4 and registered it as a fresh Bower module.  I've named it backbone.documentmodel (as opposed
to backbone-documentmodel which is the original).



[documentmodel]:		https://github.com/icereval/backbone-documentmodel
[backbonejs]:			http://backbonejs.org/
[marionette]:			http://marionettejs.com/
[myrepo]:				https://github.com/mike-alexander/backbone-documentmodel