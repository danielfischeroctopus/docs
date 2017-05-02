---
title: Use a variable to define a package feed
description: Variables can be used to define a package feed, this guide will show you how.
position: 0
version: "[3.0,4.0)"
---

When defining a package feed in Octopus, you have the option to use a variable by selecting the Custom binding option. This is often useful when the package feed needs to change based on scoping. There is something to keep in mind though when using a variable to define the package feed. At the time of release creation there is only a small amount of variable evaluation we do. And unfortunately we do not have any environmental context at this stage of the deployment. So Octopus requires a placeholder that points to

As Octopus checks the feed and package at release creation time, even if it is not used later on, we require an unscoped variable with the feed value to be present for us to evaluate.

To fix this, would you be able to do the following:
Create a new variable with the name as your feed variable and have it with out a value or scope. You should end up with 2 variables with the same name, one empty and the other with NuGet feed value.

Below are some screenshots that illustrate an example of this:


