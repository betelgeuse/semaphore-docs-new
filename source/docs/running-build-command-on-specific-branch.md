---
layout: post
title: Running a build command on specific branch
category: Customizing your build
---

Yes. Since the environment variable BRANCH_NAME is [available](/docs/available-environment-variables.html), you can add a new build command to your project settings such as:

```bash
if [ "$BRANCH_NAME" = "acceptance-tests" ]; then bundle exec rake spec:acceptance ; fi
```
