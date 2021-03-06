<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@firebase/firestore](./firestore.md) &gt; [lite](./firestore_lite.md) &gt; [CollectionReference](./firestore_lite.collectionreference.md) &gt; [withConverter](./firestore_lite.collectionreference.withconverter.md)

## CollectionReference.withConverter() method

Applies a custom data converter to this CollectionReference, allowing you to use your own custom model objects with Firestore. When you call [addDoc()](./firestore_.adddoc.md) with the returned `CollectionReference` instance, the provided converter will convert between Firestore data and your custom type `U`<!-- -->.

<b>Signature:</b>

```typescript
withConverter<U>(converter: FirestoreDataConverter<U>): CollectionReference<U>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  converter | [FirestoreDataConverter](./firestore_lite.firestoredataconverter.md)<!-- -->&lt;U&gt; | Converts objects to and from Firestore. |

<b>Returns:</b>

[CollectionReference](./firestore_lite.collectionreference.md)<!-- -->&lt;U&gt;

A `CollectionReference<U>` that uses the provided converter.

