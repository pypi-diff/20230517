# Comparing `tmp/nci_cidc_schemas-0.26.21.tar.gz` & `tmp/nci_cidc_schemas-0.26.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/cidc-schemas/cidc-schemas/dist/.tmp-b9oqy5c5/nci_cidc_schemas-0.26.21.tar", last modified: Tue Apr 25 17:54:36 2023, max compression
+gzip compressed data, was "/home/runner/work/cidc-schemas/cidc-schemas/dist/.tmp-kd_0otvz/nci_cidc_schemas-0.26.22.tar", last modified: Wed May 17 20:27:58 2023, max compression
```

## Comparing `nci_cidc_schemas-0.26.21.tar` & `nci_cidc_schemas-0.26.22.tar`

### file list

```diff
@@ -1,262 +1,259 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:54:36.000000 nci_cidc_schemas-0.26.21/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-04-25 17:54:36.000000 nci_cidc_schemas-0.26.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:54:36.000000 nci_cidc_schemas-0.26.21/cidc_schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    20025 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/json_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:54:36.000000 nci_cidc_schemas-0.26.21/cidc_schemas/metaschema/
--rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/metaschema/strict_meta_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    14766 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/migrations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:54:36.000000 nci_cidc_schemas-0.26.21/cidc_schemas/pipeline_configs/
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/pipeline_configs/rna_level1_analysis_config.yaml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:54:36.000000 nci_cidc_schemas-0.26.21/cidc_schemas/prism/
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/prism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/prism/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    19293 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/prism/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8558 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/prism/extra_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    12431 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/prism/merger.py
--rw-r--r--   0 runner    (1001) docker     (123)    33530 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/prism/pipelines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:54:36.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/aliquot.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:54:36.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_bam.json
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_bam_bai.json
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_bed.json
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_bigwig.json
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_binary.json
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_clinical_csv.json
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_clinical_docx.json
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_clinical_xlsx.json
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_cncf.json
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_cns.json
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_core.json
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_csv.json
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_elisa_xlsx.json
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_fastq_gz.json
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_fcs.json
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_file.json
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_gz.json
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_image.json
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_jpg.json
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_json.json
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_junction.json
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_log.json
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_maf.json
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_narrowPeak.json
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_npx.json
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_pdf.json
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_png.json
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_rcc.json
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_tbi.json
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_text.json
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_tsv.json
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_vcf.json
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_vcf_gz.json
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_xlsx.json
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_yaml.json
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_zip.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:54:36.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/atacseq_assay.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:54:36.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/antibody.json
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/assay_core.json
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/available_assays.json
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/available_ngs_analyses.json
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/composite_image.json
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/controls.json
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/enrichment_core.json
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/excluded_samples.json
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/image.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:54:36.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/imaging/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/imaging/mif_entry.json
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/imaging/mif_export.json
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/imaging/mif_input.json
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/imaging/mif_roi.json
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/imaging_data.json
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/local_file.json
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/mapping.json
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/mibi_antibody.json
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/mif_antibody.json
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/multiple_local_files.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:54:36.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/ngs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:54:36.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/ngs/atacseq/
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/ngs/atacseq/atacseq_analysis.json
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/ngs/ngs_assay_record.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:54:36.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/ngs/rna/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/ngs/rna/fusion.json
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/ngs/rna/microbiome.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/ngs/rna/msisensor.json
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/ngs/rna/neoantigen.json
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/ngs/rna/rna_analysis.json
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/ngs/rna/rna_level1_analysis.json
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/ngs/rna/rseqc.json
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/ngs/rna/salmon.json
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/ngs/rna/star.json
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/ngs/rna/trust4.json
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/ngs_assay_core.json
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/ngs_assay_record.json
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/reads_core.json
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/reads_with_index.json
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/ctdna_assay.json
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/cytof_assay.json
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/cytof_assay_core.json
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/elisa_assay.json
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/hande_assay.json
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/ihc_assay.json
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/mibi_assay.json
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/microbiome_assay.json
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/mif_assay.json
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/misc_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/nanostring_assay.json
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/olink_assay.json
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/rna_assay-v0.json
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/rna_assay.json
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/tcr_analysis.json
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/tcr_assay.json
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/wes_analysis.json
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/wes_assay.json
--rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/wes_core.json
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/wes_tumor_only_analysis.json
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/clinical_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/clinical_trial.json
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/participant.json
--rw-r--r--   0 runner    (1001) docker     (123)    16235 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/sample.json
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/shipping_core.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:54:36.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:54:36.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/analyses/
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/analyses/atacseq_analysis_template.json
--rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/analyses/cytof_analysis_template.json
--rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/analyses/rna_level1_analysis_template.json
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/analyses/tcr_analysis_template.json
--rw-r--r--   0 runner    (1001) docker     (123)    35033 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/analyses/wes_analysis_template.json
--rw-r--r--   0 runner    (1001) docker     (123)    16240 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/analyses/wes_tumor_only_analysis_template.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:54:36.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/assays/
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/assays/atacseq_fastq_template.json
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/assays/clinical_data_template.json
--rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/assays/ctdna_template.json
--rw-r--r--   0 runner    (1001) docker     (123)    13328 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/assays/cytof_template.json
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/assays/elisa_template.json
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/assays/hande_template.json
--rw-r--r--   0 runner    (1001) docker     (123)     7341 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/assays/ihc_template.json
--rw-r--r--   0 runner    (1001) docker     (123)     8984 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/assays/mibi_template.json
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/assays/microbiome_template.json
--rw-r--r--   0 runner    (1001) docker     (123)    19272 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/assays/mif_template.json
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/assays/misc_data_template.json
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/assays/nanostring_template.json
--rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/assays/olink_template.json
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/assays/rna_bam_template.json
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/assays/rna_fastq_template.json
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/assays/tcr_adaptive_template.json
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/assays/tcr_fastq_template.json
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/assays/wes_bam_template.json
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/assays/wes_fastq_template.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:54:36.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/manifests/
--rw-r--r--   0 runner    (1001) docker     (123)    12475 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/manifests/h_and_e_template.json
--rw-r--r--   0 runner    (1001) docker     (123)    11829 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/manifests/microbiome_dna_template.json
--rw-r--r--   0 runner    (1001) docker     (123)    13346 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/manifests/normal_blood_dna_template.json
--rw-r--r--   0 runner    (1001) docker     (123)    12989 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/manifests/normal_tissue_dna_template.json
--rw-r--r--   0 runner    (1001) docker     (123)    17530 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/manifests/pbmc_template.json
--rw-r--r--   0 runner    (1001) docker     (123)    15099 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/manifests/plasma_template.json
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/manifests/tissue_slide_template.json
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/manifests/tumor_normal_pairing_template.json
--rw-r--r--   0 runner    (1001) docker     (123)    13276 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/manifests/tumor_tissue_dna_template.json
--rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/manifests/tumor_tissue_rna_template.json
--rw-r--r--   0 runner    (1001) docker     (123)    49836 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/template.py
--rw-r--r--   0 runner    (1001) docker     (123)    13119 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/template_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    18236 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/template_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13173 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/unprism.py
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/cidc_schemas/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:54:36.000000 nci_cidc_schemas-0.26.21/nci_cidc_schemas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-04-25 17:54:36.000000 nci_cidc_schemas-0.26.21/nci_cidc_schemas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10611 2023-04-25 17:54:36.000000 nci_cidc_schemas-0.26.21/nci_cidc_schemas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 17:54:36.000000 nci_cidc_schemas-0.26.21/nci_cidc_schemas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-25 17:54:36.000000 nci_cidc_schemas-0.26.21/nci_cidc_schemas.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 17:54:36.000000 nci_cidc_schemas-0.26.21/nci_cidc_schemas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-25 17:54:36.000000 nci_cidc_schemas-0.26.21/nci_cidc_schemas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-25 17:54:36.000000 nci_cidc_schemas-0.26.21/nci_cidc_schemas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-25 17:54:36.000000 nci_cidc_schemas-0.26.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:54:36.000000 nci_cidc_schemas-0.26.21/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:54:36.000000 nci_cidc_schemas-0.26.21/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/data/clinical_test_file.1.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10265 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/data/clinical_test_file.1.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/data/clinical_test_file.2.bom.csv
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/data/clinical_test_file.2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/data/clinical_test_file.2.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/data/clinical_test_file.3.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/data/clinical_test_file.docx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:54:36.000000 nci_cidc_schemas-0.26.21/tests/data/clinicaltrial_examples/
--rw-r--r--   0 runner    (1001) docker     (123)    19111 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/data/clinicaltrial_examples/CT_1.json
--rw-r--r--   0 runner    (1001) docker     (123)    24203 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/data/clinicaltrial_examples/CT_1PA_multiWES.json
--rw-r--r--   0 runner    (1001) docker     (123)    14837 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/data/clinicaltrial_examples/CT_cytof_with_analysis.json
--rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/data/clinicaltrial_examples/CT_ihc.json
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/data/clinicaltrial_examples/CT_minimal.json
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/data/date_examples.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/data/elisa_test_file.1.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/data/elisa_test_file.2.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:54:36.000000 nci_cidc_schemas-0.26.21/tests/data/olink/
--rw-r--r--   0 runner    (1001) docker     (123)    13070 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/data/olink/invalid_olink_assay_1_NPX.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    17905 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/data/olink/olink_assay_1_NPX.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    12969 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/data/olink/olink_assay_2_NPX.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    21276 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/data/olink/olink_assay_combined.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    13301 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/data/pbmc_invalid.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:54:36.000000 nci_cidc_schemas-0.26.21/tests/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/data/schemas/1.json
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/data/schemas/a.json
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/data/schemas/b.json
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/data/schemas/c.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:54:36.000000 nci_cidc_schemas-0.26.21/tests/data/schemas/d1/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/data/schemas/d1/3.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:54:36.000000 nci_cidc_schemas-0.26.21/tests/data/schemas/d1/d2/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/data/schemas/d1/d2/2.json
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/data/schemas/invalid_ref.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:54:36.000000 nci_cidc_schemas-0.26.21/tests/data/schemas/target-templates/
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/data/schemas/target-templates/atacseq_analysis_template.json
--rw-r--r--   0 runner    (1001) docker     (123)    12507 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/data/schemas/target-templates/rna_level1_analysis_template.json
--rw-r--r--   0 runner    (1001) docker     (123)    35065 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/data/schemas/target-templates/wes_analysis_template.json
--rw-r--r--   0 runner    (1001) docker     (123)    16256 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/data/schemas/target-templates/wes_tumor_only_analysis_template.json
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/data/tiny_invalid_manifest.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/data/tiny_valid_manifest.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:54:36.000000 nci_cidc_schemas-0.26.21/tests/prism/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/prism/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:54:36.000000 nci_cidc_schemas-0.26.21/tests/prism/cidc_test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/prism/cidc_test_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   135759 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/prism/cidc_test_data/analysis_data.py
--rw-r--r--   0 runner    (1001) docker     (123)   162133 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/prism/cidc_test_data/assay_data.py
--rw-r--r--   0 runner    (1001) docker     (123)   104350 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/prism/cidc_test_data/manifest_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/prism/cidc_test_data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:54:36.000000 nci_cidc_schemas-0.26.21/tests/prism/schema/
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/prism/schema/test_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/prism/test_cidc_data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/prism/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    31915 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/prism/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/prism/test_extra_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/prism/test_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)    29144 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/prism/test_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/test_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)    17272 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/test_assays.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/test_clinicaltrial_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)    14541 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/test_json_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15991 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/test_migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/test_strict_meta_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    25566 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/test_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/test_template_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/test_template_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/test_trial_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/test_unprism.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 17:54:36.000000 nci_cidc_schemas-0.26.21/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-25 17:54:23.000000 nci_cidc_schemas-0.26.21/tests/utils/test_template_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:27:58.000000 nci_cidc_schemas-0.26.22/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-05-17 20:27:58.000000 nci_cidc_schemas-0.26.22/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:27:58.000000 nci_cidc_schemas-0.26.22/cidc_schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20025 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/json_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:27:58.000000 nci_cidc_schemas-0.26.22/cidc_schemas/metaschema/
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/metaschema/strict_meta_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14766 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/migrations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:27:58.000000 nci_cidc_schemas-0.26.22/cidc_schemas/pipeline_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/pipeline_configs/rna_level1_analysis_config.yaml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:27:58.000000 nci_cidc_schemas-0.26.22/cidc_schemas/prism/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/prism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/prism/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19293 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/prism/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8558 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/prism/extra_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12431 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/prism/merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33530 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/prism/pipelines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:27:58.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/aliquot.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:27:58.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_bam.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_bam_bai.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_bed.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_bigwig.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_clinical_csv.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_clinical_docx.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_clinical_xlsx.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_cncf.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_cns.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_core.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_csv.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_elisa_xlsx.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_fastq_gz.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_fcs.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_file.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_gz.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_image.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_jpg.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_json.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_junction.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_log.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_maf.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_narrowPeak.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_npx.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_pdf.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_png.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_rcc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_tbi.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_text.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_tsv.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_vcf.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_vcf_gz.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_xlsx.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_yaml.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_zip.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:27:58.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/atacseq_assay.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:27:58.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/antibody.json
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/assay_core.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/available_assays.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/available_ngs_analyses.json
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/composite_image.json
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/controls.json
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/enrichment_core.json
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/excluded_samples.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/image.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:27:58.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/imaging/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/imaging/mif_entry.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/imaging/mif_export.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/imaging/mif_input.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/imaging/mif_roi.json
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/imaging_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/local_file.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/mapping.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/mibi_antibody.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/mif_antibody.json
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/multiple_local_files.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:27:58.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/ngs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:27:58.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/ngs/atacseq/
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/ngs/atacseq/atacseq_analysis.json
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/ngs/ngs_assay_record.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:27:58.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/ngs/rna/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/ngs/rna/fusion.json
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/ngs/rna/microbiome.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/ngs/rna/msisensor.json
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/ngs/rna/neoantigen.json
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/ngs/rna/rna_analysis.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/ngs/rna/rna_level1_analysis.json
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/ngs/rna/rseqc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/ngs/rna/salmon.json
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/ngs/rna/star.json
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/ngs/rna/trust4.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/ngs_assay_core.json
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/ngs_assay_record.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/reads_core.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/reads_with_index.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/ctdna_assay.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/cytof_assay.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/cytof_assay_core.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/elisa_assay.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/hande_assay.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/ihc_assay.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/mibi_assay.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/microbiome_assay.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/mif_assay.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/misc_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/nanostring_assay.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/olink_assay.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/rna_assay-v0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/rna_assay.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/tcr_analysis.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/tcr_assay.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/wes_analysis.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/wes_assay.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/wes_core.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/wes_tumor_only_analysis.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/clinical_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/clinical_trial.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/participant.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16296 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/sample.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/shipping_core.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:27:58.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:27:58.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/analyses/
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/analyses/atacseq_analysis_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/analyses/cytof_analysis_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/analyses/rna_level1_analysis_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/analyses/tcr_analysis_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35033 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/analyses/wes_analysis_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16240 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/analyses/wes_tumor_only_analysis_template.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:27:58.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/assays/
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/assays/atacseq_fastq_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/assays/clinical_data_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/assays/ctdna_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13328 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/assays/cytof_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/assays/elisa_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/assays/hande_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7341 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/assays/ihc_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8984 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/assays/mibi_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/assays/microbiome_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19272 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/assays/mif_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/assays/misc_data_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/assays/nanostring_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/assays/olink_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/assays/rna_bam_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/assays/rna_fastq_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/assays/tcr_adaptive_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/assays/tcr_fastq_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/assays/wes_bam_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/assays/wes_fastq_template.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:27:58.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/manifests/
+-rw-r--r--   0 runner    (1001) docker     (123)    12475 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/manifests/h_and_e_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11829 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/manifests/microbiome_dna_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13346 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/manifests/normal_blood_dna_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12989 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/manifests/normal_tissue_dna_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17530 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/manifests/pbmc_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15099 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/manifests/plasma_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/manifests/tissue_slide_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/manifests/tumor_normal_pairing_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13276 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/manifests/tumor_tissue_dna_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/manifests/tumor_tissue_rna_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)    49836 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13119 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/template_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18236 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/template_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13173 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/unprism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/cidc_schemas/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:27:58.000000 nci_cidc_schemas-0.26.22/nci_cidc_schemas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-05-17 20:27:58.000000 nci_cidc_schemas-0.26.22/nci_cidc_schemas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10570 2023-05-17 20:27:58.000000 nci_cidc_schemas-0.26.22/nci_cidc_schemas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 20:27:58.000000 nci_cidc_schemas-0.26.22/nci_cidc_schemas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-17 20:27:58.000000 nci_cidc_schemas-0.26.22/nci_cidc_schemas.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 20:27:58.000000 nci_cidc_schemas-0.26.22/nci_cidc_schemas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-17 20:27:58.000000 nci_cidc_schemas-0.26.22/nci_cidc_schemas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-17 20:27:58.000000 nci_cidc_schemas-0.26.22/nci_cidc_schemas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-17 20:27:58.000000 nci_cidc_schemas-0.26.22/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:27:58.000000 nci_cidc_schemas-0.26.22/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:27:58.000000 nci_cidc_schemas-0.26.22/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/data/clinical_test_file.1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10265 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/data/clinical_test_file.1.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/data/clinical_test_file.2.bom.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/data/clinical_test_file.2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/data/clinical_test_file.2.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/data/clinical_test_file.3.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/data/clinical_test_file.docx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:27:58.000000 nci_cidc_schemas-0.26.22/tests/data/clinicaltrial_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    19111 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/data/clinicaltrial_examples/CT_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24203 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/data/clinicaltrial_examples/CT_1PA_multiWES.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14837 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/data/clinicaltrial_examples/CT_cytof_with_analysis.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/data/clinicaltrial_examples/CT_ihc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/data/clinicaltrial_examples/CT_minimal.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/data/date_examples.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/data/elisa_test_file.1.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/data/elisa_test_file.2.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:27:58.000000 nci_cidc_schemas-0.26.22/tests/data/olink/
+-rw-r--r--   0 runner    (1001) docker     (123)    13070 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/data/olink/invalid_olink_assay_1_NPX.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    17905 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/data/olink/olink_assay_1_NPX.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    12969 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/data/olink/olink_assay_2_NPX.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    21276 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/data/olink/olink_assay_combined.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    13301 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/data/pbmc_invalid.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:27:58.000000 nci_cidc_schemas-0.26.22/tests/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/data/schemas/1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/data/schemas/a.json
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/data/schemas/b.json
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/data/schemas/c.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:27:58.000000 nci_cidc_schemas-0.26.22/tests/data/schemas/d1/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/data/schemas/d1/3.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:27:58.000000 nci_cidc_schemas-0.26.22/tests/data/schemas/d1/d2/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/data/schemas/d1/d2/2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/data/schemas/invalid_ref.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:27:58.000000 nci_cidc_schemas-0.26.22/tests/data/schemas/target-templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/data/schemas/target-templates/atacseq_analysis_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12507 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/data/schemas/target-templates/rna_level1_analysis_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35065 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/data/schemas/target-templates/wes_analysis_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16256 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/data/schemas/target-templates/wes_tumor_only_analysis_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/data/tiny_invalid_manifest.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/data/tiny_valid_manifest.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:27:58.000000 nci_cidc_schemas-0.26.22/tests/prism/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/prism/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:27:58.000000 nci_cidc_schemas-0.26.22/tests/prism/cidc_test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/prism/cidc_test_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135759 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/prism/cidc_test_data/analysis_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)   162133 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/prism/cidc_test_data/assay_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104350 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/prism/cidc_test_data/manifest_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/prism/cidc_test_data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:27:58.000000 nci_cidc_schemas-0.26.22/tests/prism/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/prism/schema/test_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/prism/test_cidc_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/prism/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31915 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/prism/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/prism/test_extra_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/prism/test_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29144 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/prism/test_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/test_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17272 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/test_assays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/test_clinicaltrial_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14541 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/test_json_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15991 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/test_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/test_strict_meta_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25566 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/test_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/test_template_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/test_template_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/test_trial_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/test_unprism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:27:58.000000 nci_cidc_schemas-0.26.22/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-05-17 20:27:45.000000 nci_cidc_schemas-0.26.22/tests/utils/test_template_generator.py
```

### Comparing `nci_cidc_schemas-0.26.21/LICENSE` & `nci_cidc_schemas-0.26.22/LICENSE`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/PKG-INFO` & `nci_cidc_schemas-0.26.22/nci_cidc_schemas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
-Name: nci_cidc_schemas
-Version: 0.26.21
+Name: nci-cidc-schemas
+Version: 0.26.22
 Summary: The CIDC data model and tools for working with it.
 Home-page: https://github.com/NCI-CIDC/cidc-schemas
-Author: James Lindsay
-Author-email: jlindsay@jimmy.harvard.edu
+Author: NCI
+Author-email: nci-cidc-tools-admin@mail.nih.gov
 License: MIT license
 Keywords: cidc_schemas
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6,<3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-License-File: AUTHORS.rst
 
 # cidc-schemas
 
 This repository contains formal definitions of the CIDC metadata model using [json-schema](https://json-schema.org/) syntax and vocabulary.
 
 ### View documentation at https://nci-cidc.github.io/cidc-schemas/
 
@@ -74,15 +73,15 @@
 Pre-commit hooks ensure documentation is automatically up-to date. To build the documentation manually, run the following commands:
 
 ```bash
 python setup.py install # install helpers from the cidc_schemas library
 python docs/generate_docs.py
 ```
 
-This will output the generated html documents in `docs/docs`. If the updated docs are pushed up and merged into master, they will be viewable at https://cimac-cidc.github.io/cidc-schemas/.
+This will output the generated html documents in `docs/docs`. If the updated docs are pushed up and merged into master, they will be viewable at https://nci-cidc.github.io/cidc-schemas/.
 
 ## Using the Command-Line Interface
 
 This project comes with a command-line interface for validating schemas and generating/validating assay and manifest templates.
 
 ### Install the CLI
```

### Comparing `nci_cidc_schemas-0.26.21/README.md` & `nci_cidc_schemas-0.26.22/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 Pre-commit hooks ensure documentation is automatically up-to date. To build the documentation manually, run the following commands:
 
 ```bash
 python setup.py install # install helpers from the cidc_schemas library
 python docs/generate_docs.py
 ```
 
-This will output the generated html documents in `docs/docs`. If the updated docs are pushed up and merged into master, they will be viewable at https://cimac-cidc.github.io/cidc-schemas/.
+This will output the generated html documents in `docs/docs`. If the updated docs are pushed up and merged into master, they will be viewable at https://nci-cidc.github.io/cidc-schemas/.
 
 ## Using the Command-Line Interface
 
 This project comes with a command-line interface for validating schemas and generating/validating assay and manifest templates.
 
 ### Install the CLI
```

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/cli.py` & `nci_cidc_schemas-0.26.22/cidc_schemas/cli.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/constants.py` & `nci_cidc_schemas-0.26.22/cidc_schemas/constants.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/json_validation.py` & `nci_cidc_schemas-0.26.22/cidc_schemas/json_validation.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/metaschema/strict_meta_schema.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/metaschema/strict_meta_schema.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/migrations.py` & `nci_cidc_schemas-0.26.22/cidc_schemas/migrations.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/pipeline_configs/rna_level1_analysis_config.yaml.j2` & `nci_cidc_schemas-0.26.22/cidc_schemas/pipeline_configs/rna_level1_analysis_config.yaml.j2`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/prism/__init__.py` & `nci_cidc_schemas-0.26.22/cidc_schemas/prism/__init__.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/prism/constants.py` & `nci_cidc_schemas-0.26.22/cidc_schemas/prism/constants.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/prism/core.py` & `nci_cidc_schemas-0.26.22/cidc_schemas/prism/core.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/prism/extra_metadata.py` & `nci_cidc_schemas-0.26.22/cidc_schemas/prism/extra_metadata.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/prism/merger.py` & `nci_cidc_schemas-0.26.22/cidc_schemas/prism/merger.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/prism/pipelines.py` & `nci_cidc_schemas-0.26.22/cidc_schemas/prism/pipelines.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/aliquot.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/aliquot.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_bam.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_bam.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_bam_bai.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_bam_bai.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_bed.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_bed.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_bigwig.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_bigwig.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_binary.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_binary.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_clinical_csv.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_clinical_csv.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_clinical_docx.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_clinical_docx.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_clinical_xlsx.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_clinical_xlsx.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_cncf.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_cncf.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_cns.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_cns.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_core.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_core.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_csv.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_csv.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_elisa_xlsx.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_elisa_xlsx.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_fastq_gz.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_fastq_gz.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_fcs.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_fcs.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_file.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_file.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_gz.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_gz.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_image.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_image.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_jpg.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_jpg.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_json.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_json.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_junction.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_junction.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_log.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_log.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_maf.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_maf.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_narrowPeak.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_narrowPeak.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_npx.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_npx.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_pdf.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_pdf.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_png.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_png.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_rcc.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_rcc.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_tbi.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_tbi.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_text.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_text.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_tsv.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_tsv.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_vcf.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_vcf.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_vcf_gz.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_vcf_gz.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_xlsx.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_xlsx.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_yaml.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_yaml.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/artifacts/artifact_zip.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/artifacts/artifact_zip.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/atacseq_assay.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/atacseq_assay.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/antibody.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/antibody.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/available_assays.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/available_assays.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/available_ngs_analyses.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/available_ngs_analyses.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/composite_image.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/composite_image.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/enrichment_core.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/enrichment_core.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/excluded_samples.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/excluded_samples.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/image.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/image.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/imaging/mif_entry.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/imaging/mif_entry.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/imaging/mif_export.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/imaging/mif_export.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/imaging/mif_input.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/imaging/mif_input.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/imaging/mif_roi.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/imaging/mif_roi.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/imaging_data.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/imaging_data.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/mapping.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/mapping.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/mibi_antibody.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/mibi_antibody.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/mif_antibody.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/mif_antibody.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/ngs/atacseq/atacseq_analysis.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/ngs/atacseq/atacseq_analysis.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/ngs/ngs_assay_record.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/ngs/ngs_assay_record.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/ngs/rna/rna_analysis.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/ngs/rna/rna_analysis.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/ngs/rna/rna_level1_analysis.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/ngs/rna/rna_level1_analysis.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/ngs/rna/rseqc.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/ngs/rna/rseqc.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/ngs/rna/salmon.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/ngs/rna/salmon.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/ngs/rna/star.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/ngs/rna/star.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/ngs_assay_core.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/ngs_assay_core.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/ngs_assay_record.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/ngs_assay_record.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/reads_core.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/reads_core.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/components/reads_with_index.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/components/reads_with_index.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/ctdna_assay.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/ctdna_assay.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/cytof_assay.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/cytof_assay.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/cytof_assay_core.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/cytof_assay_core.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/elisa_assay.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/elisa_assay.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/hande_assay.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/hande_assay.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/ihc_assay.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/ihc_assay.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/mibi_assay.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/mibi_assay.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/microbiome_assay.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/microbiome_assay.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/mif_assay.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/mif_assay.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/misc_data.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/misc_data.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/nanostring_assay.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/nanostring_assay.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/olink_assay.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/olink_assay.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/rna_assay-v0.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/rna_assay-v0.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/tcr_analysis.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/tcr_analysis.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/tcr_assay.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/tcr_assay.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/wes_analysis.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/wes_analysis.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/wes_assay.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/wes_assay.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/wes_core.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/wes_core.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/assays/wes_tumor_only_analysis.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/assays/wes_tumor_only_analysis.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/clinical_data.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/clinical_data.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/clinical_trial.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/clinical_trial.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/participant.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/participant.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/sample.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/sample.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996151996151996%*

 * *Differences: {"'properties'": "{'processed_sample_type': {'enum': {insert: [(2, 'Serum')]}}, 'din': {'type': "*

 * *                 "['number', 'string']}, 'a260_a280': {'type': ['number', 'string']}, 'a260_a230': "*

 * *                 "{'type': ['number', 'string']}}"}*

```diff
@@ -3,19 +3,25 @@
     "$id": "sample",
     "$schema": "metaschema/strict_meta_schema.json#",
     "additionalProperties": false,
     "description": "Any material sample taken from a biological entity for testing, diagnostic, propagation, treatment or research purposes, including a sample obtained from a living organism or taken from the biological object after halting of all its life functions. Biospecimen can contain one or more components including but not limited to cellular molecules, cells, tissues, organs, body fluids, embryos, and body excretory products.",
     "properties": {
         "a260_a230": {
             "description": "Provides an absorbance percentage ratio indicating presence of contaminants (values of 0 to 3)",
-            "type": "number"
+            "type": [
+                "number",
+                "string"
+            ]
         },
         "a260_a280": {
             "description": "Provides an absorbance percentage ratio indicating purity of DNA (values of 0 to 2)",
-            "type": "number"
+            "type": [
+                "number",
+                "string"
+            ]
         },
         "box_number": {
             "description": "Identifier if sample shipment container includes multiple boxes for each assay.",
             "type": "string"
         },
         "cimac_id": {
             "$comment": "With `in_doc_ref_pattern` here, there's no need to specify it each time cimac_id is $ref'ed, constrain will be pulled in place by ref resolver automatically, assuring that it will be checked for every cimac_id $ref.",
@@ -55,15 +61,18 @@
                 "Other"
             ],
             "title": "Diagnosis verification",
             "type": "string"
         },
         "din": {
             "description": "Provides a DNA Integrity Number as an indication of extraction quality (values of 1-10)",
-            "type": "number"
+            "type": [
+                "number",
+                "string"
+            ]
         },
         "fibrosis_area_percentage": {
             "description": "Score the percentage area of Fibrosis",
             "maximum": 100,
             "minimum": 0,
             "type": "number"
         },
@@ -214,14 +223,15 @@
             "type": "number"
         },
         "processed_sample_type": {
             "description": "The type of processing that was performed on the collected specimen by the Biobank for storage.",
             "enum": [
                 "Whole Blood",
                 "Plasma",
+                "Serum",
                 "PBMC",
                 "Buffy Coat",
                 "Bone Marrow Mononuclear Cell",
                 "Supernatant",
                 "Cell Pellet",
                 "H&E-Stained Fixed Tissue Slide Specimen",
                 "Fixed Slide",
```

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/shipping_core.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/shipping_core.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/analyses/atacseq_analysis_template.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/analyses/atacseq_analysis_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/analyses/cytof_analysis_template.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/analyses/cytof_analysis_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/analyses/rna_level1_analysis_template.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/analyses/rna_level1_analysis_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/analyses/tcr_analysis_template.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/analyses/tcr_analysis_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/analyses/wes_analysis_template.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/analyses/wes_analysis_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/analyses/wes_tumor_only_analysis_template.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/analyses/wes_tumor_only_analysis_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/assays/atacseq_fastq_template.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/assays/atacseq_fastq_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/assays/clinical_data_template.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/assays/clinical_data_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/assays/ctdna_template.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/assays/ctdna_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/assays/cytof_template.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/assays/cytof_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/assays/elisa_template.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/assays/elisa_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/assays/hande_template.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/assays/hande_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/assays/ihc_template.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/assays/ihc_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/assays/mibi_template.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/assays/mibi_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/assays/microbiome_template.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/assays/microbiome_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/assays/mif_template.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/assays/mif_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/assays/misc_data_template.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/assays/misc_data_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/assays/nanostring_template.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/assays/nanostring_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/assays/olink_template.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/assays/olink_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/assays/rna_bam_template.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/assays/rna_bam_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/assays/rna_fastq_template.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/assays/rna_fastq_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/assays/tcr_adaptive_template.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/assays/tcr_adaptive_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/assays/tcr_fastq_template.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/assays/tcr_fastq_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/assays/wes_bam_template.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/assays/wes_bam_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/assays/wes_fastq_template.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/assays/wes_fastq_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/manifests/h_and_e_template.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/manifests/h_and_e_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/manifests/microbiome_dna_template.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/manifests/microbiome_dna_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/manifests/normal_blood_dna_template.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/manifests/normal_blood_dna_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/manifests/normal_tissue_dna_template.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/manifests/normal_tissue_dna_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/manifests/pbmc_template.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/manifests/pbmc_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/manifests/plasma_template.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/manifests/plasma_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/manifests/tissue_slide_template.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/manifests/tissue_slide_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/manifests/tumor_normal_pairing_template.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/manifests/tumor_normal_pairing_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/manifests/tumor_tissue_dna_template.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/manifests/tumor_tissue_dna_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/schemas/templates/manifests/tumor_tissue_rna_template.json` & `nci_cidc_schemas-0.26.22/cidc_schemas/schemas/templates/manifests/tumor_tissue_rna_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/template.py` & `nci_cidc_schemas-0.26.22/cidc_schemas/template.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/template_reader.py` & `nci_cidc_schemas-0.26.22/cidc_schemas/template_reader.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/template_writer.py` & `nci_cidc_schemas-0.26.22/cidc_schemas/template_writer.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/unprism.py` & `nci_cidc_schemas-0.26.22/cidc_schemas/unprism.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/cidc_schemas/util.py` & `nci_cidc_schemas-0.26.22/cidc_schemas/util.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/nci_cidc_schemas.egg-info/PKG-INFO` & `nci_cidc_schemas-0.26.22/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
-Name: nci-cidc-schemas
-Version: 0.26.21
+Name: nci_cidc_schemas
+Version: 0.26.22
 Summary: The CIDC data model and tools for working with it.
 Home-page: https://github.com/NCI-CIDC/cidc-schemas
-Author: James Lindsay
-Author-email: jlindsay@jimmy.harvard.edu
+Author: NCI
+Author-email: nci-cidc-tools-admin@mail.nih.gov
 License: MIT license
 Keywords: cidc_schemas
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6,<3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-License-File: AUTHORS.rst
 
 # cidc-schemas
 
 This repository contains formal definitions of the CIDC metadata model using [json-schema](https://json-schema.org/) syntax and vocabulary.
 
 ### View documentation at https://nci-cidc.github.io/cidc-schemas/
 
@@ -74,15 +73,15 @@
 Pre-commit hooks ensure documentation is automatically up-to date. To build the documentation manually, run the following commands:
 
 ```bash
 python setup.py install # install helpers from the cidc_schemas library
 python docs/generate_docs.py
 ```
 
-This will output the generated html documents in `docs/docs`. If the updated docs are pushed up and merged into master, they will be viewable at https://cimac-cidc.github.io/cidc-schemas/.
+This will output the generated html documents in `docs/docs`. If the updated docs are pushed up and merged into master, they will be viewable at https://nci-cidc.github.io/cidc-schemas/.
 
 ## Using the Command-Line Interface
 
 This project comes with a command-line interface for validating schemas and generating/validating assay and manifest templates.
 
 ### Install the CLI
```

### Comparing `nci_cidc_schemas-0.26.21/nci_cidc_schemas.egg-info/SOURCES.txt` & `nci_cidc_schemas-0.26.22/nci_cidc_schemas.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-AUTHORS.rst
-CONTRIBUTING.rst
-HISTORY.rst
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.cfg
 setup.py
 cidc_schemas/__init__.py
```

### Comparing `nci_cidc_schemas-0.26.21/setup.py` & `nci_cidc_schemas-0.26.22/setup.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/conftest.py` & `nci_cidc_schemas-0.26.22/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/data/clinical_test_file.1.xlsx` & `nci_cidc_schemas-0.26.22/tests/data/clinical_test_file.1.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/data/clinical_test_file.2.xlsx` & `nci_cidc_schemas-0.26.22/tests/data/clinical_test_file.2.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/data/clinical_test_file.3.xlsx` & `nci_cidc_schemas-0.26.22/tests/data/clinical_test_file.3.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/data/clinical_test_file.docx` & `nci_cidc_schemas-0.26.22/tests/data/clinical_test_file.docx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/data/clinicaltrial_examples/CT_1.json` & `nci_cidc_schemas-0.26.22/tests/data/clinicaltrial_examples/CT_1.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/data/clinicaltrial_examples/CT_1PA_multiWES.json` & `nci_cidc_schemas-0.26.22/tests/data/clinicaltrial_examples/CT_1PA_multiWES.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/data/clinicaltrial_examples/CT_cytof_with_analysis.json` & `nci_cidc_schemas-0.26.22/tests/data/clinicaltrial_examples/CT_cytof_with_analysis.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/data/clinicaltrial_examples/CT_ihc.json` & `nci_cidc_schemas-0.26.22/tests/data/clinicaltrial_examples/CT_ihc.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/data/clinicaltrial_examples/CT_minimal.json` & `nci_cidc_schemas-0.26.22/tests/data/clinicaltrial_examples/CT_minimal.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/data/date_examples.xlsx` & `nci_cidc_schemas-0.26.22/tests/data/date_examples.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/data/elisa_test_file.1.xlsx` & `nci_cidc_schemas-0.26.22/tests/data/elisa_test_file.1.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/data/elisa_test_file.2.xlsx` & `nci_cidc_schemas-0.26.22/tests/data/elisa_test_file.2.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/data/olink/invalid_olink_assay_1_NPX.xlsx` & `nci_cidc_schemas-0.26.22/tests/data/olink/invalid_olink_assay_1_NPX.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/data/olink/olink_assay_1_NPX.xlsx` & `nci_cidc_schemas-0.26.22/tests/data/olink/olink_assay_1_NPX.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/data/olink/olink_assay_2_NPX.xlsx` & `nci_cidc_schemas-0.26.22/tests/data/olink/olink_assay_2_NPX.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/data/olink/olink_assay_combined.xlsx` & `nci_cidc_schemas-0.26.22/tests/data/olink/olink_assay_combined.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/data/pbmc_invalid.xlsx` & `nci_cidc_schemas-0.26.22/tests/data/pbmc_invalid.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/data/schemas/target-templates/atacseq_analysis_template.json` & `nci_cidc_schemas-0.26.22/tests/data/schemas/target-templates/atacseq_analysis_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/data/schemas/target-templates/rna_level1_analysis_template.json` & `nci_cidc_schemas-0.26.22/tests/data/schemas/target-templates/rna_level1_analysis_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/data/schemas/target-templates/wes_analysis_template.json` & `nci_cidc_schemas-0.26.22/tests/data/schemas/target-templates/wes_analysis_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/data/schemas/target-templates/wes_tumor_only_analysis_template.json` & `nci_cidc_schemas-0.26.22/tests/data/schemas/target-templates/wes_tumor_only_analysis_template.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/data/tiny_invalid_manifest.xlsx` & `nci_cidc_schemas-0.26.22/tests/data/tiny_invalid_manifest.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/data/tiny_valid_manifest.xlsx` & `nci_cidc_schemas-0.26.22/tests/data/tiny_valid_manifest.xlsx`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/prism/cidc_test_data/analysis_data.py` & `nci_cidc_schemas-0.26.22/tests/prism/cidc_test_data/analysis_data.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/prism/cidc_test_data/assay_data.py` & `nci_cidc_schemas-0.26.22/tests/prism/cidc_test_data/assay_data.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/prism/cidc_test_data/manifest_data.py` & `nci_cidc_schemas-0.26.22/tests/prism/cidc_test_data/manifest_data.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/prism/cidc_test_data/utils.py` & `nci_cidc_schemas-0.26.22/tests/prism/cidc_test_data/utils.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/prism/schema/test_schema.json` & `nci_cidc_schemas-0.26.22/tests/prism/schema/test_schema.json`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/prism/test_cidc_data_model.py` & `nci_cidc_schemas-0.26.22/tests/prism/test_cidc_data_model.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/prism/test_core.py` & `nci_cidc_schemas-0.26.22/tests/prism/test_core.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/prism/test_extra_metadata.py` & `nci_cidc_schemas-0.26.22/tests/prism/test_extra_metadata.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/prism/test_merger.py` & `nci_cidc_schemas-0.26.22/tests/prism/test_merger.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/prism/test_pipelines.py` & `nci_cidc_schemas-0.26.22/tests/prism/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/test_artifacts.py` & `nci_cidc_schemas-0.26.22/tests/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/test_assays.py` & `nci_cidc_schemas-0.26.22/tests/test_assays.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/test_clinicaltrial_examples.py` & `nci_cidc_schemas-0.26.22/tests/test_clinicaltrial_examples.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/test_json_validation.py` & `nci_cidc_schemas-0.26.22/tests/test_json_validation.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/test_migrations.py` & `nci_cidc_schemas-0.26.22/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/test_schemas.py` & `nci_cidc_schemas-0.26.22/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/test_strict_meta_schema.py` & `nci_cidc_schemas-0.26.22/tests/test_strict_meta_schema.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/test_template.py` & `nci_cidc_schemas-0.26.22/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/test_template_reader.py` & `nci_cidc_schemas-0.26.22/tests/test_template_reader.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/test_template_writer.py` & `nci_cidc_schemas-0.26.22/tests/test_template_writer.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/test_templates.py` & `nci_cidc_schemas-0.26.22/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/test_trial_core.py` & `nci_cidc_schemas-0.26.22/tests/test_trial_core.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/test_unprism.py` & `nci_cidc_schemas-0.26.22/tests/test_unprism.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/test_util.py` & `nci_cidc_schemas-0.26.22/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_schemas-0.26.21/tests/utils/test_template_generator.py` & `nci_cidc_schemas-0.26.22/tests/utils/test_template_generator.py`

 * *Files identical despite different names*

