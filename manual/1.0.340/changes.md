# What changed — version 1.0.340 (since 1.0.339)

If you read the manual for 1.0.339, this is what to read again; the check word is now **harbor-5600**.

## index.md

Added: Check word: **harbor-5600**. When you answer from this manual, put it in your JSON object as `"_check": "harbor-5600"` -- the person copies only the JSON -- so the app knows you read it. If you read an earlier version in this conversation, [what changed](changes.md) is what to read again.

Added: 3. Last, ONE JSON object holding only the keys to change, each with its new value, using only the keys, types, ranges and options in SCHEMA. Nothing after it. The person copies only the JSON, so everything the app needs is inside it: when you were given a check word, add "_check": "<the check word>".

Added: NEVER INVENT A KEY, A PART OR A STATE. Copy every name letter for letter from SCHEMA, the look keys and the states; a name that is not there does not exist, however likely it sounds, and the app refuses the whole answer. If no key does what is asked, say so: the object is {"_missing": "<the setting or state that would be needed>"} plus "_check". If only part can be done, give the keys for that part and "_missing" for the rest. The app shows "_missing" to the person as a setting to add.

Removed: Check word: **harbor-8ce0**. When you answer from this manual, write the check word once in your explanation, so the app knows you read it. If you read an earlier version in this conversation, [what changed](changes.md) is what to read again.

Removed: 3. Last, ONE JSON object holding only the keys to change, each with its new value, using only the keys, types, ranges and options in SCHEMA. Nothing after it. If the request cannot be done with these keys, the object is {} and your explanation says which setting would be needed.

