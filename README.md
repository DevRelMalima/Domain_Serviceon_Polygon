## [Article Idea Generator](https://www.articleideagenerator.com/)

This simple tool generates article ideas for your blog or website. It's a great way to get started with your content marketing strategy.

[![Article Idea Generator](./public/screenshot.png)](https://www.articleideagenerator.com/)
[![Article Idea Generator](./public/screenshot-2.png)](https://www.articleideagenerator.com/)

## How to use

1. Go to [https://domain-serviceon-polygon.vercel.app/](https://domain-serviceon-polygon.vercel.app/)
2. Click on Connect wallet to connect your wallet and switch to mumbai
3. Enter the domain you want to mint, provide the Domain description, and click 'mint' to continue
4. Your domain will show as the recent mint domain on the dashboard
5. Click on the Domain to see your digital representation of the domain on opensea testnet


## How it works

The [OpenAI GPT-3 API](https://openai.com/api/) (text-davinci-003) and [Vercel Edge streaming](https://vercel.com/features/edge-functions) features are used in this application. Based on the user's input, it creates a prompt, sends it to the GPT-3 API using a Vercel Edge function, and streams the response back to the application.

## Running Project Locally

1. Fork the repo
2. Clone the repo
3. After cloning the repo, go to [OpenAI](https://beta.openai.com/account/api-keys) to make an account and generate your API key
4. Rename the `.env.example` file on the root of the project to `.env`, then paste your API key in the `.env` file
5. Run `npm install` to install all the dependencies
6. Run `npm run dev` to start the project
7. Go to [http://localhost:3000](http://localhost:3000) to see the project running

## Contributing

If you want to contribute to this project, please read the [contributing guide](./CONTRIBUTING.md). If you have any ideas or suggestions, feel free to open an issue or a pull request. 

If you like this project, please give it a star ⭐️


## Contributors 💪

Thanks for spending your time helping `Article Idea Generator` grow. Happy Hacking 🍻

[![Contributors](https://contrib.rocks/image?repo=Olanetsoft/article-idea-generator)](https://github.com/Olanetsoft/article-idea-generator/edit/main/README.md)

## Stargazers ⭐️

[![Stargazers](https://git-lister.onrender.com/api/stars/Olanetsoft/article-idea-generator?limit=15)](https://github.com/Olanetsoft/article-idea-generator)


## Acknowledgement

Built with 💗 by [Olanetsoft](https://twitter.com/olanetsoft) & [Kelvin](https://twitter.com/iam_kelvinjnr). Inspired by [Nutlope](https://twitter.com/nutlope), powered by [Open AI](https://openai.com/) & [Vercel Edge Functions](https://vercel.com).
