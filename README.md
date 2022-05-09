# Pandoc PLOS ONE sample reproduction. 

Use pandoc to reproduce sample manuscript for PLOS ONE journal.   
See [PLOS ONE Submission Guidelines](https://journals.plos.org/plosone/s/submission-guidelines).
  
- [doc_without_ref](doc_without_ref) : a sample manuscript without reference.
- [doc_with_ref](doc_with_ref) : a sample manuscript with reference. 

### To convert a document

For both case, you need to install 
- Pandoc
- Pantable
- pandoc-mustache
- pandoc-docx-pagebreak-py
- pandoc-crossref

and just run to create document. 
```
pandoc -d default.yaml
```

For a manuscript with reference, I already prepared bibText style of references 
`1_plosone.bib` and citation syle language `plos-one.csl`, 
so that you can convert markdon to docx. 

In sum, all you need to do is, 
- Install above packages.
- Prepare default.yaml (already provided in this repository).
- Prepare `variables.yaml`. (Empty is ok, or remove pandoc-mustache)
- Write markdown.
- Prepare bib style references and citation style language, and specify these paths in `default.yaml`. 

That's all!

