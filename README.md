# SignatureLib
Library for creating signature view on screen

**Include the following view in xml and you are ready to get the signature view in your xml.**

```xml
<com.raos.signature.Signature
        android:layout_width="match_parent"
        android:layout_height="match_parent" />
```

**Clearing the canvas for re-signing: clear() method clear the witten signature on the canvas.**

```java
import com.raos.signature.Signature;

void clear() {
  mSignatureView.clear();
}
```

**Saving the signature to a file.**

```java

/**
 * 
 * @param signatureView - Signature view which is included in xml.
 * @param filePath - File path to which the signature should be savde to.
 */
void save(View signatureView, String filePath) {
  mSignatureView.save(signatureView, filePath);
}
```
