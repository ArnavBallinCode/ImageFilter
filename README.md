# BMPImageFilter

This project is a simple command-line tool that applies various filters to BMP image files. The filters include grayscale, sepia, reflection, and blur. It is implemented in C and uses the BMP file format.

## Files
- **Makefile**: Instructions to compile the program using `clang`.
- **bmp.h**: Defines data structures for handling BMP file headers and pixels.
- **filter.c**: Contains the main function that handles command-line arguments and applies the chosen filter.
- **helpers.c**: Implements the different image filters.
- **helpers.h**: Header file declaring the functions implemented in `helpers.c`.

## Filters
- **Grayscale**: Converts the image to shades of gray.
- **Sepia**: Applies a sepia tone to the image.
- **Reflection**: Reflects the image horizontally.
- **Blur**: Applies a blur effect to the image.

## Usage
Compile the program using the Makefile:
```bash
make filter
```

Run the program:
```bash
./filter [filter_flag] infile.bmp outfile.bmp
```

### Filter Flags
- `-b`: Blur
- `-g`: Grayscale
- `-r`: Reflection
- `-s`: Sepia

### Example
To apply a sepia filter to an image:
```bash
./filter -s infile.bmp outfile.bmp
```

## Notes
- The program only supports 24-bit uncompressed BMP 4.0 files.
- Ensure that your input file is in the correct format before using the tool.

## License
This project is licensed under the MIT License.
```

### File Names
- **Main Program**: `filter.c`
- **Helper Functions**: `helpers.c` and `helpers.h`

### Instructions for Uploading to GitHub
1. Create a new repository named **BMPImageFilter** on GitHub.
2. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/ArnavBallinCode/BMPImageFilter.git
   ```
3. Navigate to the repository directory:
   ```bash
   cd BMPImageFilter
   ```
4. Copy the provided files (`Makefile`, `bmp.h`, `filter.c`, `helpers.c`, `helpers.h`) to the repository directory.
5. Create the `README.md` file with the content provided above.
6. Add and commit the files:
   ```bash
   git add .
   git commit -m "Initial commit with BMP image filters"
   ```
7. Push the changes to GitHub:
   ```bash
   git push origin main
   ```
