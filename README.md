## Responsibility

This only contains the generic gitlab-ci file to be included in another repos, it can be done like this:


```

include: 'https://gitlab.gog.com/gitlab-ci-config/blob/master/base-gitlab-ci.yml'

someTask:
  script:
    - some script

```

## IMPORTANT
Any extra configuration, like extra files to publish-please or other libraries, has to be included independently in each
repo according to it's needs.
This only works for copying a centralized text file so we all run the same jobs in the pipelines.
