---
layout: post
title: "Use std::lock_guard when possible"
date: 2021-10-03 21:09:00 +1100
tags: C++
published: true
---

Use `std::lock_guard` when possible.

`std::lock_guard` is a RAII style lock that when current scope exit, the lock will automatically release, avoiding leaving mutex to be locked if exception occur in current scope.