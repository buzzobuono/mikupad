# mikupad

**mikupad** is a lightweight and efficient language model front-end powered by ReactJS, all packed into a single HTML file. This project is inspired by the likes of NovelAI and provides a simple yet powerful interface for generating text with the help of various backends.

## Features

* **Multiple Backends**: Multiple backends are supported, namely **llama.cpp**, **koboldcpp**, and any other backend with **OpenAI compatible** APIs. You can seamlessly switch between these backends to get different text generation experiences.
* **Session Persistence**: Your text generation sessions are automatically saved and restored. This means you can work on your text in multiple sittings and continue right where you left off. Import and export your sessions to share your creative work or switch devices effortlessly.
* **Persistent Context**:
  * **Memory**: Seamlessly inject a text of your choice at the beginning of the context.
  * **Author's Note**: Seamlessly inject a text of your choice at the end of the context, with adjustable depth.
  * **World Info**: Dynamically include extra information in the context, triggered by specific keywords.
* **Prediction Undo/Redo**: It's possible to undo and redo predictions, making it easy to experiment and fine-tune your generated text until it's just right.
* **Token Probability** *(llamacpp/openai backend)*: When you hover over a token in the generated text, a list will show at most 10 tokens with their probabilities. This information can be a valuable aid in refining your text. Moreover, you can click on another token's probability to restart text generation from that point.
  * If you're using oobabooga, make sure to use an _HF sampler for this feature to function properly.
* **Logit Bias** *(llamacpp/koboldcpp backend)*: Adjust the likelihood of certain tokens being generated on the fly.
* **Completion/Chat**: Let your model directly continue your prompt in Completion Mode, or toggle on Chat Mode to have your input be wrapped in user-defined instruct formats.
* **Themes**: Customize your environment by choosing from a variety of themes.

## Getting Started

You can easily run **mikupad** by opening the `mikupad.html` file in your web browser. No additional installation is required. Choose your preferred backend and start generating text!

```shell
git clone https://github.com/lmg-anon/mikupad.git
cd mikupad
open mikupad.html
```
To use **mikupad** fully offline, run the provided `compile` script or download the pre-compiled `mikupad_compiled.html` file from [Releases](https://github.com/lmg-anon/mikupad/releases/latest).

You can also [try it on GitHub Pages](https://lmg-anon.github.io/mikupad/mikupad.html).

## Contributing

Contributions from the open-source community are welcome. Whether it's fixing a bug, adding a feature, or improving the documentation, your contributions are greatly appreciated. To contribute to **mikupad**, follow these steps:

1. Fork the repository.
2. Create a new branch for your changes: `git checkout -b feature/your-feature-name`
3. Make your changes and commit them: `git commit -m 'Add your feature'`
4. Push your changes to your forked repository: `git push origin feature/your-feature-name`
5. Open a pull request on the main repository, explaining your changes.

## License

This project is released to the public domain under the CC0 License - see the [LICENSE](LICENSE) file for details.
