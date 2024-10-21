# Modular CV

When writing applications I always have to either submit a resume, a professional CV or an academic CV. Since it is very easy to loose track when I updated one and not the other, I wrote these little templates.

The content is in the `content.tex` file and the three templates just show what is saved there. I only need to upate the contents file and then recompile the templates and everything is up to date.



Modular CV is a collection of LaTeX templates designed to simplify the process of maintaining multiple CV formats for different purposes, such as resumes, professional CVs, and academic CVs. Managing content across these documents can often become tedious and inconsistent, so this repository offers a centralized solution.

All content is stored in a single `content.tex` file, which serves as the source of information for the templates. By updating this file, you can ensure that all CV formats reflect the latest changes, maintaining consistency across different versions. Simply recompile the templates to generate up-to-date documents tailored to your specific needs.


## How It Works

Centralized Content: All bullet points, personal details, and sections are maintained in content.tex.
Three Template Files: The repository includes three templates, each tailored to a specific CV format: Resume, Professional CV, and Academic CV.
Effortless Updates: You only need to update the content.tex file, recompile, and the changes will be applied across all templates.


## Getting Started

Clone this repository to your local machine:

```bash
    git clone https://github.com/yourusername/modular-cv.git
```

Edit the `content.tex` file to add or modify information.
Recompile the templates using your LaTeX editor of choice.
Export the resulting PDF files for submission.


## Requirements

A LaTeX distribution (e.g., TeX Live, MiKTeX) is required to compile the templates.
A LaTeX editor (e.g., TeXworks, Overleaf, or VS Code with the LaTeX Workshop extension) is recommended for editing.


## Preview

### Resume

<p align="center">
    <img alt="Screenshot" src="https://raw.githubusercontent.com/EtienneMueller/CV/main/imgs/resume.png" width="800">
</p>

### Professional

<p align="center">
    <img alt="Screenshot" src="https://raw.githubusercontent.com/EtienneMueller/CV/main/imgs/professional-0.png" width="800">
    <img alt="Screenshot" src="https://raw.githubusercontent.com/EtienneMueller/CV/main/imgs/professional-1.png" width="800">
</p>

### Academic CV

<p align="center">
    <img alt="Screenshot" src="https://raw.githubusercontent.com/EtienneMueller/CV/main/imgs/academic-0.png" width="800">
    <img alt="Screenshot" src="https://raw.githubusercontent.com/EtienneMueller/CV/main/imgs/academic-1.png" width="800">
    <img alt="Screenshot" src="https://raw.githubusercontent.com/EtienneMueller/CV/main/imgs/academic-2.png" width="800">
</p>

These .png files have been created using ImageMagick. The current version gives an error due to security policies and the line `<policy domain="coder" rights="read | write" pattern="PDF" />` has to be added to `/etc/ImageMagick-6/policy.xml`

Then, to create the image files:
```bash
convert -density 300 -alpha remove -bordercolor gray90 -border 5 -strip resume.pdf imgs/resume.png
convert -density 300 -alpha remove -bordercolor gray90 -border 5 -strip professional.pdf imgs/professional.png
convert -density 300 -alpha remove -bordercolor gray90 -border 5 -strip academic.pdf imgs/academic.png
```


## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests to improve the templates or add new features.


## License

This project is licensed under the MIT License. See the `LICENSE` file for details.
