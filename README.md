npm init -y 

npm install next

npm install react

npm install react-dom

```json
"scripts": {
  "dev": "next dev"
}
```

mkdir pages

cd pages 

touch index.tsx
```tsx
export default function Home() {
    return (
        <>
        </>
    )
}
```

npm install --save-dev typescript @types/react

./pages/_app.tsx
```tsx
import { AppProps } from 'next/app';
import Head from 'next/head';

export default function MyApp({Component, pageProps}: AppProps) {
    return (
        <>
            <Head>
                <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Roboto:300,400,500,700&display=swap" />
            </Head>
            <Component {...pageProps} />
        </>
    )
}
```
