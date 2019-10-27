`desymlink-node-modules`
========================

# Installation

	yarn add desymlink-node-modules

# Use

	# 1. update modules
	yarn
	# 2. turn symlinked modules into normal files and folders
	./node_modules/.bin/desymlink-node-modules

# Why?

React Native's [Metro bundler **cannot follow symlinks**](https://github.com/facebook/metro/issues/1).

This means that without some kind of workaround, you can't use [yarn workspaces](https://yarnpkg.com/lang/en/docs/workspaces/) with React Native.
