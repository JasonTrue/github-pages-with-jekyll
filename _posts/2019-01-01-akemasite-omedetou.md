---
title: "It's the beginning of a new year"
date: 2019-01-1
---

# It's the beginning of a new year

I hope you'll have a good one.

This is just an experiment and I hope you didn't come here looking for anything insightful.

My actual blog [Pursuing My Passions](https://blog.jagaimo.com)is ancient. I hope to write something for it by the 10 year anniversary of my last post.

Here's some random code from a personal project that I'm posting because it's only slightly embarrassing.

```ruby
  def set_date_navigation
    @by_year_and_month = @blog.posts.unscoped.group('cast(extract(year from publish_at) as integer)').group('cast(extract(month from publish_at) as integer)').order('cast(extract(year from publish_at) as integer)').order('cast(extract(month from publish_at) as integer)').count
    @by_year = @blog.posts.unscoped.group('cast(extract(year from publish_at) as integer)').order('cast(extract(year from publish_at) as integer)').count
  end
```
