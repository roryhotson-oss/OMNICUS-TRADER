# Contributing to OMNICUS TRADER \ud83e\udd16

> **"Together we hunt bigger profits."**

We welcome and encourage community contributions to OMNICUS! Whether you're a developer, trader, designer, or just passionate about AI trading, there are many ways to contribute.

---

## \u2764\ufe0f **Ways to Contribute**

### **\ud83d\udc81 Code Contributions**
- Fix bugs
- Add new features
- Improve existing code
- Add new exchange connectors
- Create new trading strategies
- Optimize performance

### **\ud83d\udcc4 Documentation**
- Improve README.md
- Write tutorials
- Add examples
- Update wiki
- Translate to other languages

### **\ud83d\udca1 Testing**
- Report bugs
- Write test cases
- Improve test coverage
- Test new features

### **\ud83d\udcac Community Support**
- Answer questions in Discord
- Help new users
- Share your strategies
- Provide feedback

### **\ud83d\udce2 Other Ways**
- Star the repository
- Share on social media
- Write blog posts
- Create video tutorials
- Donate to the project

---

## \ud83d\udc80 **Getting Started**

### **Prerequisites**

1. **Fork the repository**
   ```bash
   git fork https://github.com/roryhotson-oss/OMNICUS-TRADER.git
   ```

2. **Clone your fork**
   ```bash
   git clone https://github.com/your-username/OMNICUS-TRADER.git
   cd OMNICUS-TRADER
   ```

3. **Set up development environment**
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   pip install -r requirements.txt
   pip install -r requirements-dev.txt  # If exists
   ```

4. **Create a feature branch**
   ```bash
   git checkout -b feature/your-feature-name
   ```

---

## \ud83d\udce6 **Development Guidelines**

### **Code Style**

- Follow [PEP 8](https://peps.python.org/pep-0008/) style guide
- Use type hints (Python 3.11+)
- Add docstrings to functions and classes
- Keep line length under 100 characters
- Use consistent naming conventions

### **Testing**

- All new code must have tests
- Run existing tests before submitting
- Tests should cover edge cases
- Use pytest for testing

```bash
# Run all tests
python -m pytest tests/ -v

# Run specific test
python -m pytest tests/test_omnicus.py::test_ai_brain -v
```

### **Commits**

- Use descriptive commit messages
- Follow [Conventional Commits](https://www.conventionalcommits.org/) format
- Reference issue numbers when applicable

```bash
# Good commit messages
git commit -m "feat: add Binance futures support"
git commit -m "fix: resolve API connection timeout issue"
git commit -m "docs: update README with Docker instructions"
git commit -m "test: add unit tests for memory bank"
```

---

## \ud83d\udc8b **Pull Request Process**

### **Before Submitting**

1. **Run tests**
   ```bash
   python -m pytest tests/ -v
   ```

2. **Check code formatting**
   ```bash
   # If black is installed
   black .
   
   # If isort is installed
   isort .
   ```

3. **Update documentation**
   - Update README.md if needed
   - Add/Update relevant docs
   - Update CHANGELOG.md

4. **Squash commits** (if many small commits)
   ```bash
   git rebase -i HEAD~5
   ```

### **Submitting a PR**

1. Push your branch
   ```bash
   git push origin feature/your-feature-name
   ```

2. Open a Pull Request on GitHub
   - Go to: https://github.com/roryhotson-oss/OMNICUS-TRADER/pulls
   - Click "New Pull Request"
   - Select your fork and branch
   - Fill out the PR template

3. **PR Template**

```markdown
## Description

Brief description of what this PR does.

## Related Issue

Fixes #123 or Closes #456

## Changes Made

- Added feature X
- Fixed bug Y
- Updated documentation Z

## Testing

- [ ] All existing tests pass
- [ ] New tests added
- [ ] Manual testing completed

## Screenshots (if applicable)

![Screenshot](link-to-image)

## Notes

Any additional context or information.
```

---

## \ud83d\udc81 **Code Review Process**

### **What to Expect**

1. **Initial Review** (1-2 days)
   - Maintainers will review your PR
   - Feedback on code quality, style, and approach

2. **Request Changes** (if needed)
   - Address all feedback
   - Push new commits to the same branch

3. **Approval**
   - All tests pass
   - Code meets quality standards
   - Documentation is complete

4. **Merge**
   - Maintainer will merge your PR
   - You'll be credited as a contributor!

### **Tips for Faster Reviews**

- Keep PRs small and focused
- One feature per PR
- Include tests
- Update documentation
- Respond to feedback promptly
- Be patient and polite

---

## \ud83d\udce7 **Project Structure**

```
OMNICUS-TRADER/
├── agent/                  # AI Brain
│   ├── ai_brain.py         # Central decision engine
│   ├── memory_bank.py      # Experience learning
│   ├── emotions.py         # Emotional intelligence
│   ├── skills.py           # Trading abilities
│   ├── tools.py            # Technical indicators
│   └── workflow.py         # Orchestration
│
├── core/                   # Trading Core
│   ├── hybrid_system.py    # Main trading coordinator
│   ├── trading_agent.py    # AI execution engine
│   ├── trading_mode.py     # Mode definitions
│   ├── price_engine.py      # Technical analysis
│   └── database_manager.py # Data persistence
│
├── connectors/             # Exchange APIs
│   ├── binance_connector.py
│   ├── alpaca_connector.py
│   └── unified.py           # Unified interface
│
├── soul/                   # Personality
│   ├── personality.py      # Human-like communication
│   ├── emotions.py         # Emotional state
│   └── voice.py            # TTS alerts
│
├── api/                    # FastAPI Server
│   └── server.py           # REST API endpoints
│
├── dashboards/             # Web UI
│   └── omnicus_universal.html
│
└── tests/                  # Test Suite
    └── test_omnicus.py
```

---

## \ud83d\udc82 **Label System**

We use GitHub labels to categorize issues and PRs:

| Label | Description | Color |
|-------|-------------|-------|
| `bug` | Bug report | \ud83d\udc1e Red |
| `enhancement` | Feature request | \ud83d\udda0 Blue |
| `documentation` | Documentation improvement | \ud83d\udcd6 Green |
| `good first issue` | Good for new contributors | \ud83d\udc89 Purple |
| `help wanted` | Needs community help | \ud83d\udc8a Orange |
| `question` | Question or discussion | \u2753 Gray |
| `wontfix` | Won't be fixed | \u26aa Black |

---

## \ud83d\udce6 **Reporting Issues**

### **Before Reporting**

1. Check the [FAQ](https://github.com/roryhotson-oss/OMNICUS-TRADER/wiki/FAQ)
2. Search existing issues
3. Check the [Troubleshooting Guide](https://github.com/roryhotson-oss/OMNICUS-TRADER/wiki/Troubleshooting)

### **Issue Template**

```markdown
## Description

Clear description of the issue.

## Steps to Reproduce

1. Do this
2. Then do that
3. Observe the bug

## Expected Behavior

What should happen.

## Actual Behavior

What actually happens.

## Environment

- OS: [e.g., Ubuntu 22.04]
- Python version: [e.g., 3.11.4]
- OMNICUS version: [e.g., 1.0.0]

## Logs/Errors

```
Paste relevant error messages or logs here
```

## Additional Context

Any other information.
```

---

## \u2699 **Coding Standards**

### **Python**

```python
# Good
class AIBrain:
    """Central decision engine for OMNICUS."""
    
    def __init__(self, config: dict) -> None:
        self.config = config
        self.memory = MemoryBank()

    def generate_signal(self, context: MarketContext) -> TradeSignal:
        """Generate a trading signal."""
        # Implementation
        pass


# Bad (avoid)
class ai_brain:
    def __init__(self, c):
        self.c = c
        self.m = MemoryBank()
```

### **Imports**

```python
# Good
import asyncio
import logging
from datetime import datetime
from typing import Optional, List, Dict, Any

# Bad (avoid)
import *
from datetime import *
```

### **Error Handling**

```python
# Good
try:
    result = await self.exchange.get_price(symbol)
except ExchangeError as e:
    logger.error(f"Failed to get price for {symbol}: {e}")
    raise

# Bad (avoid)
try:
    result = await self.exchange.get_price(symbol)
except:
    pass  # Silent failure
```

---

## \ud83d\udc8e **Security Guidelines**

### **\u274c Never**
- Commit API keys or secrets
- Hardcode sensitive data
- Use `print()` for sensitive information
- Store secrets in plain text

### **\u2705 Always**
- Use environment variables for secrets
- Use `.env.example` for documentation
- Add `.env` to `.gitignore`
- Validate all user inputs
- Use HTTPS for web interfaces

---

## \ud83d\udc8f **Maintainers**

### **Current Maintainers**
- [@roryhotson](https://github.com/roryhotson-oss) - Project Lead

### **Becoming a Maintainer**

If you're consistently contributing high-quality code and helping the community, you may be invited to become a maintainer. Maintainers have:

- Write access to the repository
- Ability to merge PRs
- Ability to manage issues
- Responsibility to review contributions

---

## \u2764\ufe0f **Code of Conduct**

### **Our Pledge**

We pledge to make participation in our community a harassment-free experience for everyone, regardless of age, body size, visible or invisible disability, ethnicity, sex characteristics, gender identity and expression, level of experience, education, socio-economic status, nationality, personal appearance, race, religion, or sexual identity and orientation.

### **Our Standards**

Examples of behavior that contributes to a positive environment for our community include:

- Demonstrating empathy and kindness toward other people
- Being respectful of differing opinions, viewpoints, and experiences
- Giving and gracefully accepting constructive feedback
- Accepting responsibility and apologizing to those affected by our mistakes
- Focusing on what is best not just for us as individuals, but for the overall community

Examples of unacceptable behavior include:

- The use of sexualized language or imagery
- Trolling, insulting, or derogatory comments
- Public or private harassment
- Publishing others' private information without explicit permission
- Other conduct which could reasonably be considered inappropriate in a professional setting

### **Enforcement**

Project maintainers are responsible for clarifying and enforcing our standards of acceptable behavior and will take appropriate and fair corrective action in response to any behavior that they deem inappropriate, threatening, offensive, or harmful.

---

## \ud83d\udc8d **Acknowledgments**

Thank you to all contributors who have helped make OMNICUS better:

- [List of contributors](https://github.com/roryhotson-oss/OMNICUS-TRADER/graphs/contributors)

---

## \u2728 **Resources**

- [Python Documentation](https://docs.python.org/3/)
- [PEP 8 Style Guide](https://peps.python.org/pep-0008/)
- [Conventional Commits](https://www.conventionalcommits.org/)
- [GitHub Docs](https://docs.github.com/)
- [OMNICUS Discord](https://discord.gg/omnicus)

---

## \ud83d\ude80 **Ready to Contribute?**

1. **Fork** the repository
2. **Clone** your fork
3. **Code** your feature
4. **Test** thoroughly
5. **Submit** a Pull Request

**Together we make OMNICUS the best AI trading system in the world!** \ud83e\udd16

---

*\u2764\ufe0f Thank you for contributing to OMNICUS TRADER*
