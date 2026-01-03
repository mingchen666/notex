# Changelog

All notable changes to this project will be documented in this file.

## [Unreleased]

### Added
- **Infographic Transformation**: A new feature to transform text content into visually appealing infographics.
  - Integration with **Google Gemini Nano Banana** SDK.
  - Support for `gemini-3-pro-image-preview` model for image generation.
  - Expert visualization prompts for hand-drawn/illustration style designs.
  - Full Chinese language support for infographic labels and descriptions.
  - Dedicated UI container for rendering generated infographics in the note view.
- **Enhanced Logging**: Integrated `github.com/kataras/golog` for professional, leveled logging across the application.
- **Configuration**: Added `GOOGLE_API_KEY` environment variable support for Google AI services.

### Changed
- **Migration to golog**: Replaced standard library `log` and `fmt.Printf` with `golog` for better observability and structured output.
- **UI Update**: Added "Infographic" card to the STUDIO panel in the workspace.
- **Documentation**: Updated `README.md`, `README_CN.md`, and `.env.example` with new feature details and configuration instructions.

### Fixed
- Improved response handling for image generation using `GenerateContent` and `InlineData`.
- Fixed potential 404 errors by using verified model names and API versions.
- Cleaned up unused imports and refined build process.
