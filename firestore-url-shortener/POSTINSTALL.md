This mod listens to the Cloud Firestore collection `${param:COLLECTION_PATH}`, then shortens any URL added to the field `${param:URL_FIELD_NAME}` in any document within that collection.

This mod shortens the URL then saves it in the `${param:SHORT_URL_FIELD_NAME}` field of the same document like so:

```
{
  ${param:URL_FIELD_NAME}: 'https://my.super.long-link.com/api/user/profile/-jEHitne10395-k3593085',
  ${param:SHORT_URL_FIELD_NAME}: 'https://bit.ly/EKDdza',
}
```

If the original URL in a document is updated, then the shortened URL will be automatically updated, too.