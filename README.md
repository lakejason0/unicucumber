<div align="center">

<img src="https://raw.githubusercontent.com/SkyEye-FAST/unicucumber/master/public/icon.png">

<h1>UniCucumber</h1>

</div>

This is a project for editing Unifont glyphs in browsers.

See [*Unifoundry.com* Unifont Utilities](https://unifoundry.com/unifont/unifont-utilities.html) for more information.

## Demostration

You can try the demo at the following links:

- <https://unicucumber.vercel.app/>
- <https://uni.lakeus.xyz/>

## Features

- [x] Responsive web design
- [x] Mouse and touchscreen support
- [x] Undo and redo actions
- [ ] Copy and paste actions (TODO)
- Multiple glyphs support
  - [x] A screen to list multiple glyphs
  - [x] Glyph search and filter
- Hexadecimal format support
  - [x] Export single glyph as hexadecimal string
  - [x] Import single glyph from hexadecimal string
  - [x] Save and load multiple glyphs in `.hex` format
- Image support
  - [x] Export single glyph as images (PNG, BMP, SVG, etc.)
  - [x] Import glyphs from image files
  - [ ] Generate bitmaps like `unihex2bmp` in Unifont Utilities (TODO)
- Font support
  - [ ] Export multiple glyphs as an OpenType font file (TODO)

## Usage

To use this project, you need to have Node.js installed on your computer. Then, follow these steps:

1. Clone this repository:

    ``` shell
    git clone https://github.com/SkyEye-FAST/unicucumber.git
    ```

2. Install dependencies:

    ``` shell
    cd unicucumber
    npm install
    ```

3. Start the development server:

    ``` shell
    npm run dev
    ```

4. Open your browser and go to `http://localhost:5173/`.
