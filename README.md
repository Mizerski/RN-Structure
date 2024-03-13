## The Directory Structure
Here is a bird's eye view of the recommended directory structure:

```
Project
  -src
    |--- assets
    |--- screens
    |--- navigation
    |--- services
    |--- components
    |--- hooks
    |--- types
    |--- redux
    |--- utils
```

## Assets
The assets directory is where you should put all your static assets, such as fonts and images. It's a good idea to organize these assets into separate subdirectories for each asset type. For example:

```
assets
  |--- fonts
  |--- images
```

## Services
The services directory is where you should put all your code related to external services, such as APIs. It's a good idea to organize these services into separete subdirectories for each service type. For example:
```
services
  |--- apiclient
  |--- requestInterceptor
  |--- responseInterceptor
  |--- urls
  |--- UserApi
```
## Components
The components directory is where you should put all your reusable components. Each component should have its own directory with the following files
* index.ts: The main component file.
* ComponentName.ts: The ts file for the component.
* styles.ts: The styles for the component.
* helper.ts: Any helper functions related to the component.
* useAnimation.ts: Any animation-related hooks for the component.
  
## Hooks
The hooks directory is where you should put all your custom jooks.
Each hook should have its own file. For example:

```
hooks
  |--- useBackHandler.ts
  |--- useKeyboard.ts
```

## Utils
The utils folder contains various utility functions that are not related to a specific feature or module of the app. Here are some examples of files that might be included in this folder:
```
utils
    |--- Analytics.ts
    |--- CommonUtils.ts
    |--- Logger.ts
    |--- ErrorManager.ts
    |--- DateTimeUtils.ts
    |--- EncryptedStore.ts
    |--- string.ts
    |--- constants.ts
    |--- enums.ts
```

## Project Full
```
  -src
    |--- assets
    |      |--- fonts
    |            |--- <<Your Fonts>>
    |      |--- images
    |            |--- << Your Images>>
    |
    |
    |--- route
    |      |--- screenName
    |      |      |--- index.js
    |      |      |--- styles.ts
    |      |      |--- helper.ts
    |      |      |--- screenName.tsx
    |      |      |--- screenName.test.tsx
    |      |      |--- useAnimated.ts (Optional)
    |      |      |--- components (Optional)
    |      |
    |      |--- screenName2
    |              |--- index.js
    |              |--- styles.ts
    |              |--- helper.ts
    |              |--- screenName.tsx
    |              |--- screenName.test.tsx
    |              |--- useAnimated.ts (Optional)
    |              |--- components (Optional)
    |  
    |--- navigation
    |      |--- NavigationContainer
    |      |--- Route
    |      |--- NavigationService
    |      |--- linking
    |
    |--- networking
    |      |--- apiclient
    |      |--- requestInterceptor (Assuming axios)
    |      |--- responseInterceptor (Assuming axios)
    |      |--- urls
    |      |--- UserApi (You can create a file for a group of related api calls)
    |
    |--- components
    |      |---Button (This is will have same structure as the screen)
    |      |      |--- index.ts
    |      |      |--- Button.tsx
    |      |      |--- styles.ts
    |      |      |--- helper.ts
    |      |      |--- useAnimated.ts (Optional)
    |      |
    |      |--- <<Any other component>>
    |
    |--- hooks
    |      |--- useBackHandler.ts
    |      |--- useKeyboard.ts
    |      |--- useUploadImage.ts
    |      |--- useCamera.ts
    |      |--- <<Any other hook>>
    |
    |--- types 
    |      |--- UserInterface
    |      |--- MediaInterface
    |      |--- AppConfigInterface
    |
    |--- redux
    |      |--- store.ts
    |      |--- slices
    |            |--- UserSlice
    |            |--- IntermittentSlice
    |            |--- ToastSlice
    |
    |--- utils
    |      |--- Analytics.ts
    |      |--- CommonUtils.ts
    |      |--- Logger.ts
    |      |--- ErrorManager.ts
    |      |--- DateTimeUtils.ts
    |      |--- EncryptedStore.ts
    |      |--- string.ts
    |      |--- constants.ts
    |      |--- enums.ts
    |     
---------------------------- << MULTIPLE MODULE APP >> ----------------
    |--- Module_Name
          |--- routes
          |--- components
          |--- hooks
```
