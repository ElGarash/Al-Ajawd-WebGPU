# Whisper Web

ML-powered speech recognition directly in your browser! Built with [🤗 Transformers.js](https://github.com/xenova/transformers.js).

Check out the demo site [here](https://huggingface.co/spaces/Xenova/whisper-webgpu).

https://github.com/xenova/whisper-web/assets/26504141/5d6ed3d9-5f99-4d89-8e38-9d4fc8d5baaf

## Running locally

1. Clone the repo and install dependencies:

    ```bash
    git clone https://github.com/xenova/whisper-web.git
    cd whisper-web
    npm install
    ```

2. Run the development server:

    ```bash
    npm run dev
    ```

    > Firefox users need to change the `dom.workers.modules.enabled` setting in `about:config` to `true` to enable Web Workers.
    > Check out [this issue](https://github.com/xenova/whisper-web/issues/8) for more details.

3. Open the link (e.g., [http://localhost:5173/](http://localhost:5173/)) in your browser.

## Pushing to Hugging Face Spaces

1. build the project
    ```bash
    npm run hf-build
    ```
2. push the project to Hugging Face Spaces

    ```bash
    cd dist
    git commit # if you have made any changes
    git push # (you need to configure the ssh keys before pushing to the repo)
    ```
