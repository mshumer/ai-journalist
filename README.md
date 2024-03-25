# AI-Journalist
[![Twitter Follow](https://img.shields.io/twitter/follow/mattshumer_?style=social)](https://twitter.com/mattshumer_)

# Claude-Journalist | An experimental AI-powered journalist

Claude-Journalist leverages the power of the Claude 3 AI model to research, write, and edit high-quality articles on any given topic. It utilizes web search APIs to gather relevant information, analyzes the content, and generates well-structured, informative, and engaging articles that read as if they could be published in major media publications.

## Try it without code!
If you want to try the AI journalist, but don't want to bother with code, you can use a modified version directly on the [HyperWrite Platform](https://app.hyperwriteai.com/personalassistant/tool/183607bc-a92d-4d7b-9b7d-358b4758b2c0). If you're a first-time user, you will be asked to sign in. Once you do so, come back and click this link again to go directly to the tool.

## Workflow

- Prompts the user to enter a topic to write about
- Generates a list of search terms related to the topic using Claude 3 Haiku
- Performs searches using the SERP API for each search term
- Asks Claude to select the most relevant and informative URLs from the search results
- Retrieves the article text from the selected URLs using the `newspaper3k` library
- Asks Claude to write a high-quality article based on the retrieved article texts
- Asks an editor (Claude) to review the article and provide suggestions for improvement
- Asks the editor (Claude) to rewrite the article based on the suggestions
- Prints the generated article and the edited article

## Requirements

To run Claude-Journalist, you need:
- An Anthropic API key for accessing the Claude AI model
- A SERP API key for performing web searches

## Usage

1. Open the `claude_journalist.ipynb` notebook in Google Colab or Jupyter Notebook.
2. Replace the placeholders for `ANTHROPIC_API_KEY` and `SERP_API_KEY` in the notebook with your respective API keys.
3. Run the notebook cells sequentially to execute the code.
4. When prompted, enter the topic you want to write an article about.
5. Wait for the AI system to research, write, and edit the article.

## Disclaimer

Claude-Journalist is an experimental tool designed to assist in the article writing process. While it aims to generate high-quality content, the output should be carefully reviewed and fact-checked by human editors before any publication. The generated articles may require further editing and refinement to meet specific editorial standards and guidelines.

## License

This project is licensed under the [MIT License](LICENSE).

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

Some known improvement areas:
- Enhance the search result filtering and selection process
- Implement additional fact-checking and verification mechanisms
- Optimize the article structure and formatting

## Contact

Matt Shumer - [@mattshumer_](https://twitter.com/mattshumer_)

Lastly, if you want to try something even cooler than this, sign up for [HyperWrite Personal Assistant](https://app.hyperwriteai.com/personalassistant). It's basically an AI with access to real-time information that a) is incredible at writing naturally, and b) can operate your web browser to complete tasks for you.
