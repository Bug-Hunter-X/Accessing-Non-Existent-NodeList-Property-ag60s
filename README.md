# Accessing Non-Existent NodeList Property in HTML

This repository demonstrates an uncommon bug in HTML related to accessing non-existent properties of a NodeList.  NodeList objects returned by methods like `querySelectorAll` do not have custom properties defined by default. Attempting to access or assign them can lead to issues, mostly in how browsers handle these operations. This particular issue is subtle and might not throw an immediate error, leading to unexpected behavior.

## Bug Description
The code tries to set a property (`myNonExistentProperty`) on a NodeList, which is not a standard behavior and may cause unexpected results. The impact varies depending on the browser and its version.