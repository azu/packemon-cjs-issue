https://github.com/milesj/packemon/issues/133

    npm run build

and packemon change package.json

```diff
❯ git diff
diff --git a/package.json b/package.json
index 3939b82..9e67565 100644
--- a/package.json
+++ b/package.json
@@ -39,15 +39,13 @@
     "./*": {
       "types": "./dts/*.d.ts",
       "node": {
-        "import": "./mjs/*.mjs",
-        "require": "./cjs/*.cjs"
+        "import": "./mjs/*.mjs"
       }
     },
     ".": {
       "types": "./dts/index.d.ts",
       "node": {
-        "import": "./mjs/index.mjs",
-        "require": "./cjs/index.cjs"
+        "import": "./mjs/index.mjs"
       }
     }
   },
```
