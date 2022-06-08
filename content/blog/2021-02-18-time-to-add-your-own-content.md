---
createdAt: 2021-02-18
title: Wolf.
description:
---

```js{1,4}[posts.vue]
formatDate(dateString) {
const date = new Date(dateString)
return date.toLocaleDateString(process.env.lang) || ''
},
async fetchPosts(
  postType = this.postType,
  amount = this.amount,
  sortBy = this.sortBy,
) {
return this.$content(postType)
  .sortBy(sortBy.key, sortBy.direction)
  .limit(amount)
  .fetch()
  .catch((err) => {
    error({ statusCode: 404, message: amount > 1 ? 'Posts not found' : 'Post not found' })
  });
}
```

## Wolf

Wolf: Wolf is not a sane person but he was not always like this
he was stable with a family working his software firm
when things went sour in 08 and his only client backed out.

# and wolf... stay off the dance floor
