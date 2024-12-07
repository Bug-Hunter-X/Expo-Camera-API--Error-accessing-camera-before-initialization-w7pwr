# Expo Camera Initialization Error

This repository demonstrates a common error when using the Expo Camera API: attempting to access camera functions before the camera has finished initializing.  The `bug.js` file shows the problematic code, while `bugSolution.js` provides the corrected version.

**Problem:**  The original code tries to access camera features immediately, leading to errors.  The solution involves using the `onCameraReady` callback to ensure the camera is ready before accessing its functionalities.

**Solution:** The corrected code waits for the `onCameraReady` event before executing camera operations, preventing errors and improving app stability.