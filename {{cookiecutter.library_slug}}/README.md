{% set is_open_source = cookiecutter.open_source_license != 'Not open source' -%}
{% for _ in cookiecutter.project_name %}={% endfor %}
{{ cookiecutter.project_name }}
{% for _ in cookiecutter.project_name %}={% endfor %}

{{ cookiecutter.project_short_description }}

## Installation

Install dependencies by running `pip install -r requirements.txt`.

## Training

```bash
allennlp train experiments/venue_classifier.json -s /tmp/your_output_dir_here --include-package my_library
```

<hr/>

This project was created using [cookiecutter-allennlp](https://github.com/jacobdanovitch/cookiecutter-allennlp), which is based on [allennlp-as-a-library-example](https://github.com/allenai/allennlp-as-a-library-example).
