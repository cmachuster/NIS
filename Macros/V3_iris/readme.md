How to use it in your control script

```js
import { APERTURE_BY_REFERENCE } from "./APERTURE_BY_REFERENCE.js";

function applyApertureForObjective(objCode) {
  const aperture = APERTURE_BY_REFERENCE[objCode] ?? 70;
  Stg_SetAperturePosition(3, aperture);
}
```

This is now:
🔒 deterministic
🧪 optically consistent
🧩 easy to regenerate if the CSV changes
