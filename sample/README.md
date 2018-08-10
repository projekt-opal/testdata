# sample

This folder contains crawled raw documents and annotated metadata for the mCLOUD random sample from OPAL D1.2.

## Files

The folder contains two CSV files, `urls.csv` and `extract.csv`, along with the source files (`url_id.extension`).

### `urls.csv`

This file maps URL IDs, such as 209 (used in D1.2), to the actual URL (e.g., http://mcloud...xyz). Additionally, it has a third column "referrer" indicating the URL ID by which the crawler will be able to find that document (by following a link).

### `extract.csv`

This file contains the relevant metadata from the document. It contains the URL ID (as in `urls.csv`), the xpath and selector of the element (identified using Chrome's inspector (press F12)), a non-normative property (indicating what this field is about), the content (or a snippet), and a comment (which can be used to explain further what this metadata item is, or warn about issues). Next, the fields rdf-property and rdf-value can be used to define which vocabulary could be used to represent this metadata (and how).
