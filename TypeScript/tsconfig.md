````json
//best one
  {
    "compilerOptions": {
    "lib": ["DOM", "ES6"],
    "target": "es6",
    "rootDir": "src",
    "outDir": "dist"
  }
}
//or
```json
{
  "compilerOptions": {
    "target": "es2016",
    "module": "commonjs",
    "esModuleInterop": true,
    "forceConsistentCasingInFileNames": true,
    "strict": true,
    "skipLibCheck": true,
    "outDir": "./dist"
  },
  "include": ["src"]
}

````
