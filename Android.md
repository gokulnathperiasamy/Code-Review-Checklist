# Android Code Review Checklist

> When reviewing Android code, the reviewer might use the following checklist. In addition to below checklist, use Java-J2EE review checklist for generic Java related codereview.


1. Use updated Android Studio, Gradle and Libraries.
2. Put passwords and sensitive data in gradle.properties file.
3. Use Retrofit/Volley, Otto/EventBus and OkHttp libraries.
4. Choose between Activities and Fragments carefully.
5. Layout XMLs are organized preoperly.
6. Use styles to avoid duplicate attributes in layout XMLs.
7. Use multiple style files to avoid a single huge one
8. Keep your colors.xml short and DRY, just define the palette
9. Keep dimens.xml DRY, define generic constants
10. Do not make a deep hierarchy of ViewGroups, make use of relative layout whenever possible.
11. Avoid client-side processing for WebViews, and beware of leaks
12. Use SharedPreferences for simple persistence, otherwise ContentProviders
13. Proper localization and translation. (Localize static string in the project, don’t rely on google translate to convert to other languages.)
14. Save the app state.
15. Check for unexpected app behavior. Handle possible exceptions in the block, don’t throw any general exceptions
16. Check for app crashes, integrate crash analytics tool with the App (ACRA) or any other SDK.
17. Does app degrade gracefully in case of unknown failures?
18. Are the app level standards being followed?
19. Are the layouts suitable for all the screen dimensions?
20. Is the correct form of storage being used and is memory available for storage?
21. Are all the fail points handled?
22. How will the functionalities affect the performance of the app - time and memory? Run the profile tool to see the memory usage over the period of time.
23. Is it absolutely necessary to run it on UI therad or would a background thread suffice? Don’t run heavy task on the UI Thread, use Async Tasks to do so.
24. Can we decrease the coupling?
25. Include resources for xxxhdpi screens - decide the supported form factors and supporting icons for the best user experiences.
26. Place launcher icons in mipmap-folders.
27. Use separate resources for debug and release.
28. Use shapes and selectors instead of images as much as possible - avoid using images if there is a way to achieve through drawables/colors.
29. Use the Parcelable class instead of Serializable when passing data in Intents/Bundles.
30. Use an Retrofit/Volley instead of an AsyncTask.
31. Is file operations performed off the UI thread?
32. Is the code written following the coding standards/guidelines provided in Java Checklist?
33. Can we run unit test/debug the code easily to find the root cause?
34. Are data encrypted on the device? Is plain storing of data should be strictly avoided?
35. Use separate dimensions for multiple layout.
36. Use build flavours and type accordingly.
37. Do not hardcode signing config password in gradle file. Set it as System.Environment variables.
38. Do not hardcode URLs and API_KEYS in gradle file. Use gradle.properties file.
