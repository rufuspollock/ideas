---
created: 2019-08-29
title: Giftless - Git LFS server as a service
emoji: 🎁
status: 
status_notes: 
website: https://giftless.app/
---
Git + Cloud Storage for large files = ❤️

A simple solution for data versioning using the tools you know and love. 

Git LFS enables git to store large files outside git in the cloud. The problem is you are locked into github / gitlab and their pricey storage. With Giftless you can bring your own cloud storage like S3 / R2 etc and combine it seamlessly with your existing git repos in github, gitlab or elsewhere.
## More detail

Context ...

- Tracking data along with your code / content is really cool
- "Versioning" data (even in simple copy on write) is really desirable (and wanted - cf dvc etc)
- Git LFS lets you do this ...
- Github gives you ~ 1GB / month of git lfs storage and bandwidth

The problem ...

- Github (and gitlab) data limits are really low
- I want to use my own storage like s3, r2 etc
  - so that i can access data directly
  - i can do other data science / engineering stuff with it etc

Question: how can i still get to use git(hub) for my code, docs, content etc *and* store my data where i want (with low b/w and storage costs)?

Answer: have a git lfs gateway that allows using storage that is not github's or gitlab's but YOUR OWN ...

And guess what ... we built this in 2019-2021 in form of Giftless: https://github.com/datopian/giftless

Note: we did sketch an MVP offer for this in 2020/2021

And even posted a v early version here 

https://datahub.io/data-versioning back in 2021

![[assets/giftless-early-offer.png]]

## Other places this is up

- https://wip.co/projects/giftless