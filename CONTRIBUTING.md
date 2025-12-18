# Contributing to API Finder

Thank you for your interest in contributing to API Finder! This document provides guidelines for adding new APIs to our directory.

## How to Add an API

### Prerequisites

- A GitHub account
- Basic knowledge of Markdown
- The API you're submitting should be publicly accessible

### Step-by-Step Guide

#### 1. Fork the Repository

Click the "Fork" button at the top right of the repository page to create your own copy.

#### 2. Clone Your Fork

```bash
git clone https://github.com/YOUR_USERNAME/apifinder.git
cd apifinder
```

#### 3. Create a New Branch

```bash
git checkout -b add-api-name
```

Replace `api-name` with a descriptive name for the API you're adding.

#### 4. Add the API to README.md

Find the appropriate category section in `README.md` and add a new row to the table. Each API entry should follow this format:

```markdown
| [API Name](https://api-landing-page.com) | Brief description of what the API does | `authType` | Yes/No/Unknown | Type | [Docs](https://api-documentation-url.com) |
```

#### Table Columns Explained

| Column | Description | Valid Values |
|--------|-------------|--------------|
| **API** | Name of the API linked to its landing page | `[Name](URL)` |
| **Description** | Brief description (max 100 characters) | Text |
| **Auth** | Authentication method required | `apiKey`, `OAuth`, `No`, or other |
| **CORS** | Whether the API supports CORS | `Yes`, `No`, `Unknown` |
| **Type** | Pricing model of the API | `Free`, `Freemium`, `Paid`, `Open Source` |
| **Docs** | Link to API documentation | `[Docs](URL)` |

#### Type Values Explained

| Type | Description |
|------|-------------|
| `Free` | Completely free to use with no paid tiers |
| `Freemium` | Free tier available with paid plans for more features/usage |
| `Paid` | Requires payment to use (may have trial period) |
| `Open Source` | Open source API that you can self-host |

#### Example Entry

```markdown
| [OpenAI](https://openai.com) | GPT models, DALL-E, Whisper and more | `apiKey` | Yes | Paid | [Docs](https://platform.openai.com/docs/api-reference) |
```

#### 5. Commit Your Changes

```bash
git add README.md
git commit -m "Add [API Name] to [Category]"
```

#### 6. Push to Your Fork

```bash
git push origin add-api-name
```

#### 7. Create a Pull Request

1. Go to the original repository on GitHub
2. Click "Pull Requests" > "New Pull Request"
3. Click "compare across forks"
4. Select your fork and branch
5. Click "Create Pull Request"
6. Fill in the PR template with details about the API

## Guidelines for Submissions

### API Requirements

- **Publicly Accessible**: The API must be available for public use (free or paid)
- **Documentation**: The API must have documentation
- **Working**: The API should be active and functional
- **No Duplicates**: Check that the API isn't already listed

### Quality Standards

- **Accurate Information**: Verify all details before submitting
- **Correct Category**: Place the API in the most appropriate category
- **Concise Description**: Keep descriptions brief but informative
- **Valid Links**: Ensure both the landing page and documentation links work

### What We Accept

- Public REST APIs
- GraphQL APIs
- WebSocket APIs
- SOAP APIs (if publicly documented)

### What We Don't Accept

- Private or internal APIs
- APIs requiring special enterprise agreements to access documentation
- Deprecated or discontinued APIs
- APIs that violate GitHub's Terms of Service

## Pull Request Checklist

Before submitting your PR, please ensure:

- [ ] The API is not already in the list
- [ ] The API has public documentation
- [ ] All table columns are filled correctly
- [ ] The entry is in alphabetical order within its category
- [ ] The description is under 100 characters
- [ ] Both the API landing page link and documentation link are working
- [ ] You've selected the correct category
- [ ] The Type field accurately reflects the API's pricing model

## Adding a New Category

If you believe a new category is needed:

1. Open an issue first to discuss the new category
2. Provide examples of APIs that would fit in this category
3. Wait for approval before creating a PR

## Reporting Issues

Found a broken link or incorrect information? Please:

1. Open an issue with the title: `[Fix] API Name - Issue Description`
2. Provide details about what needs to be corrected
3. Include the correct information if known

## Code of Conduct

- Be respectful and constructive
- Help maintain a welcoming community
- Focus on the quality of contributions

## Questions?

If you have questions about contributing, feel free to open an issue with the label `question`.

---

Thank you for helping make API Finder a comprehensive resource for developers!
