# Contributing to Awesome Free Dev Tools

Thank you for your interest in contributing to Awesome Free Dev Tools! We welcome contributions that help developers discover genuinely useful free tools.

Our goal is to maintain a curated, trustworthy collection of tools that developers can actually use for free — not a directory for promoting paid products or driving upgrades to Pro plans.

## 📌 Contribution Guidelines

Before submitting a Pull Request, please ensure the tool meets the following criteria:

- **Free & Usable:** Must offer a genuinely usable free tier or be fully free and open-source. Temporary free trials alone do not qualify.
- **Useful for Developers:** Must provide practical value for software developers, such as development, debugging, testing, design, productivity, or deployment.
- **Accessible & Maintained:** The tool must be accessible, with sufficient documentation or instructions to understand its purpose and usage. Established community adoption or a minimum number of GitHub stars is not required.
- **Transparency:** Pricing, free-tier limitations, and relevant restrictions must be described accurately.
- **Self-Promotion:** Contributors may submit their own tools, provided they disclose their affiliation and the tools meet the same eligibility criteria.
- **Proper Formatting:** Place the tool in the correct category, follow the repository's data format, avoid duplicates, and regenerate generated files using the project's build script.

## How to Contribute

### Adding a New Tool

1. Check whether the tool already exists in the repository.
2. Verify that it meets the inclusion criteria above.
3. Fork the repository.
4. Add the tool to the appropriate category file in `data/tools/` (e.g., `database-backend.json`, `ai-coding-ides-agents.json`, etc.) following the existing format:

   ```json
   {
       "name": "Tool Name",
       "url": "https://example.com",
       "category": "Category Name",
       "purpose": "Brief, factual description of the free functionality",
       "pricing": "Free Tier: Describe relevant limits"
   }
   ```

   If you need to create a new category, create a new JSON file in `data/tools/` with the category name (slugified, e.g., `new-category.json`) and add the tool there.

5. Run the build script to update `README.md` and `docs/index.html`:

   ```bash
   node scripts/build-readme.js
   ```

6. Commit your changes with a descriptive message.
7. Push to your fork and submit a Pull Request.
8. Include the official pricing source, free-tier details, and any required affiliation disclosure in your Pull Request description.

### Reporting Issues

If you find a problem with an existing tool, such as a broken link, incorrect category, misleading pricing information, or a change in free-tier availability:

1. Check whether the issue has already been reported.
2. Open an issue with a clear title and description.
3. Include supporting evidence or official documentation where possible.
4. Suggest a fix if applicable.

### Suggesting Improvements

Have ideas for improving the project? We'd love to hear them!

1. Open an issue describing your suggestion.
2. Explain why the change would benefit developers.
3. Provide examples or mockups where applicable.
4. For new tool suggestions, follow the inclusion criteria and provide official pricing information and evidence of meaningful free functionality.

Suggestions that do not meet the repository's inclusion criteria may be closed without further action.

## Development Setup

1. Clone the repository.
2. Install dependencies, if any.
3. Run the build script to regenerate the documentation.

## Code of Conduct

By participating in this project, you agree to abide by our [Code of Conduct](CODE_OF_CONDUCT.md).

## License

By contributing to Awesome Free Dev Tools, you agree that your contributions will be licensed under the MIT License.
