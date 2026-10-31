STUDYAPKMOD KGS — FINAL API + PREMIUM UI PACKAGE

WHAT IS INCLUDED
- Existing frontend UI and application routes
- Premium dark-blue responsive UI stylesheet
- Batch list source priority updated to the two requested GitHub JSON files
- Course/classroom loading prioritizes api.khanglobalstudies.com/v1/courses/{id}
- Lesson/media details prioritize sahukgs.com/api/lesson/{id}
- Removed dependency on studyapkmod.free.nf proxy endpoints
- MP4/direct URL and YouTube embed fields are handled when the API actually returns them
- PDF/notes URLs are normalized when present in the API response

API FLOW
1. Batch list: https://sahuvijay143.github.io/kgs_batch_list/New_Sunny.json
2. Fallback batch list: https://sunnyji7256.github.io/kgs_batch_list/New_Sunny.json
3. Course details/classrooms: https://api.khanglobalstudies.com/v1/courses/{id}
4. Lesson/media details: https://sahukgs.com/api/lesson/{id}

DEPLOY TO VERCEL
1. Extract the ZIP.
2. Upload the contents to the root of a GitHub repository; index.html must be in the root.
3. Import the repository in Vercel.
4. Select Other as framework preset.
5. Use no build command and set output directory to . for this static package.
6. Deploy.

IMPORTANT LIMITATIONS
- This package is a static frontend. It does not include a separate private backend source code.
- Browser access to external APIs depends on the source server's CORS policy and availability.
- Existing verification features are preserved in the frontend, but authoritative verification requires the matching backend routes to remain available.
- Video playback depends on valid media URLs returned by the source API, supported formats, and source-server permissions.
- The API response fields could not be fully verified during packaging; the frontend accepts common response shapes but must be tested against live responses.
- No API access control, DRM, or authentication restrictions are bypassed.
