[![DOI](https://zenodo.org/badge/235376482.svg)](https://zenodo.org/badge/latestdoi/235376482)


# Repetitions-Expander
Script that expands the repetition marks, such as repetition bars, Da Capo or Dal Segno, in a MusicXML score.

Copy the file in your project directory and include it in your main script. Given a MusicXML score opened with Music21, a possible execution example would be:

```python
repeat_elements = get_repeat_elements(score)
expanded_score = expand_score_repetitions(score, repeat_elements)
```

The first line returns a list containing all the repeat elements and the bar where they are found. For instance: `[('Segno', 17), ('Dal Segno', 50)]`. While the second line returns a complete music21 score.
