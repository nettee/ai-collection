# YC guide to vibe coding

YC 合伙人 Tom Blomfield 分享的 Vibe Coding 技巧。

> * 原文链接：https://www.youtube.com/watch?v=BJjsfNO5JTo
> * 译文与解析：可前往我的[公众号文章](https://mp.weixin.qq.com/s/oHLGJZF_pSUAMpNW7yLxBw)阅读

## Planning process

*   **Create a comprehensive plan**: Start by working with the AI to write a detailed implementation plan in a markdown file
*   **Review and refine**: Delete unnecessary items, mark features as won't do if too complex
*   **Maintain scope control**: Keep a separate section for ideas for later to stay focused
*   **Implement incrementally**: Work section by section rather than attempting to build everything at once
*   **Track progress**: Have the AI mark sections as complete after successful implementation
*   **Commit regularly**: Ensure each working section is committed to Git before moving to the next

## Version control strategies

*   **Use Git religiously**: Don't rely solely on the AI tools' revert functionality
*   **Start clean**: Begin each new feature with a clean Git slate
*   **Reset when stuck**: Use git reset --hard HEAD if the AI goes on a vision quest
*   **Avoid cumulative problems**: Multiple failed attempts create layers and layers of bad code
*   **Clean implementation**: When you finally find a solution, reset and implement it cleanly

## Testing framework

*   **Prioritize high-level tests**: Focus on end-to-end integration tests over unit tests
*   **Simulate user behavior**: Test features by simulating someone clicking through the site/app
*   **Catch regressions**: LLMs often make unnecessary changes to unrelated logic
*   **Test before proceeding**: Ensure tests pass before moving to the next feature
*   **Use tests as guardrails**: Some founders recommend starting with test cases to provide clear boundaries

## Effective bug fixing

*   **Leverage error messages**: Simply copy-pasting error messages is often enough for the AI
*   **Analyze before coding**: Ask the AI to consider multiple possible causes
*   **Reset after failures**: Start with a clean slate after each unsuccessful fix attempt
*   **Implement logging**: Add strategic logging to better understand what's happening
*   **Switch models**: Try different AI models when one gets stuck
*   **Clean implementation**: Once you identify the fix, reset and implement it on a clean codebase

## AI tool optimization

*   **Create instruction files**: Write detailed instructions for your AI in appropriate files (cursor.rules, windsurf.rules, claude.md)
*   **Local documentation**: Download API documentation to your project folder for accuracy
*   **Use multiple tools**: Some founders run both Cursor and Windsurf simultaneously on the same project
*   **Tool specialization**: Cursor is a bit faster for frontend work, while Windsurf think slonger
*   **Compare outputs**: Generate multiple solutions and pick the best one

## Complex feature development

*   **Create standalone prototypes**: Build complex features in a clean codebase first
*   **Use reference implementations**: Point the AI to working examples to follow
*   **Clear boundaries**: Maintain consistent external APIs while allowing internal changes
*   **Modular architecture**: Service-based architectures with clear boundaries work better than monorepos

## Tech stack considerations

*   **Established frameworks excel**: Ruby on Rails works well due to 20 years of consistent conventions
*   **Training data matters**: Newer languages like Rust or Elixir may have less training data
*   **Modularity is key**: Small, modular files are easier for both humans and AIs to work with
*   **Avoid large files**: Don't have files that are thousands of lines long

## Beyond coding

*   **DevOps automation**: Use AI for configuring servers, DNS, and hosting
*   **Design assistance**: Generate favicons and other design elements
*   **Content creation**: Draft documentation and marketing materials
*   **Educational tool**: Ask the AI to explain implementations line by line
*   **Use screenshots**: Share UI bugs or design inspiration visually
*   **Voice input**: Tools like Aqua enable 140 words per minute input

## Continuous improvement

*   **Regular refactoring**: Once tests are in place, refactor frequently
*   **Identify opportunities**: Ask the AI to find refactoring candidates
*   **Stay current**: Try every new model release
*   **Recognize strengths**: Different models excel at different tasks