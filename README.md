#s3-remote-storage

It's like a `localStorage`, but not `local`.
This library offers you a kind of "BaaS" solution, to use S3 Bucket as a remote storage tool for JSON data.

### Methods

`init` - initialize S3 bucket environment.
For example:

```javascript
import S3RemoteStorage from "s3-remote-storage";

S3RemoteStorage.init(
  ACCESS_KEY_ID,
  SECRET_ACCESS_KEY,
  BUCKET_NAME,
  BUCKET_REGION
);
```

`setItem` - Add a item to the bucket.
For example:

```javascript
import S3RemoteStorage from "s3-remote-storage";

const data = S3RemoteStorage.setItem("fooBar", { foo: "bar" });

console.log("Response content:", data);
```

`getItem` - Add a item from the bucket.
For example:

```javascript
import S3RemoteStorage from "s3-remote-storage";

const data = S3RemoteStorage.getItem("fooBar");

console.log("Response content:", data);
```

`removeItem` - Remove a item from the bucket.
For example:

```javascript
import S3RemoteStorage from "s3-remote-storage";

const data = S3RemoteStorage.removeItem("fooBar");

console.log("Response content:", data);
```
