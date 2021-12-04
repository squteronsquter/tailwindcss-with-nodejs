# Install Tailwind CSS with Node

```
mkdir tw
cd tw
npm init -y
npm install tailwindcss
```

## Create two folders

```
mkdir src public
```

# Create css file which will hold tailwind to be processed

```
touch src/styles.css
```

## Place tailwind inside

```
@tailwind base;
@tailwind components;
@tailwind utilities;
```

## Tweak your package.json file to be able to use a script to process tailwind

```
[...]
"scripts": {
    "build-css": "tailwindcss build src/styles.css -o public/styles.css"
  },
[...]
```
## Run the script to process css for the first time

```
npm run build-css
```

## Reprocess everytime you make changes to src/styles.css

## To configure or tweak configuration of tailwind

```
npx tailwindcss init --full
```

## Rename the created tailwind.config.js file to something else to have access to default classes and generate a new empty config file

```
npx tailwindcss init
```

## Tweak your tailwindcss inside this file

## Rebuild css

```
npm run build-css
```


## That is it!

