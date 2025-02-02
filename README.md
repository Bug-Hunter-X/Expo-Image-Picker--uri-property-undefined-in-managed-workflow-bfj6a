# Expo Image Picker: uri property undefined in managed workflow

This repository demonstrates a bug encountered when using the `expo-image-picker` library within an Expo managed workflow project.  The problem lies in the inconsistency of the `uri` property of the selected image.  Sometimes it's correctly populated with the image's URI; other times, it's `undefined`, causing unexpected application behavior.

The `bug.js` file showcases the problematic code. The `bugSolution.js` file provides a potential solution by introducing a check for the `uri` property before use. Note that this might not be a permanent fix.  Further investigation into Expo's managed workflow and its interaction with the image picker library is needed.

**Reproducing the Bug:**

1. Clone this repository.
2. Install dependencies: `npm install` or `yarn install`.
3. Run the project in an Expo managed workflow environment.
4. Select an image using the image picker.
5. Observe that the `uri` property might be `undefined` on certain attempts, leading to errors.