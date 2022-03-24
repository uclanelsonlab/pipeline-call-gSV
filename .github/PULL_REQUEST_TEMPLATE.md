<!--- Please read each of the following items and confirm by replacing
 !--the [ ] with a [X] --->

- [ ] I have read the [code review guidelines](https://confluence.mednet.ucla.edu/display/BOUTROSLAB/Code+Review+Guidelines) and the [code review best practice on GitHub check-list](https://confluence.mednet.ucla.edu/pages/viewpage.action?pageId=84091668).

- [ ] I have set up the branch protection rule following the [github standards](https://confluence.mednet.ucla.edu/pages/viewpage.action?spaceKey=BOUTROSLAB&title=GitHub+Standards#GitHubStandards-Branchprotectionrule) before opening this pull request, or the branch protection rule has already been set up.

- [ ] I have added my name to the contributors listings in the
``metadata.yaml`` and the ``manifest`` block in the config as part of this pull request, am listed
already, or do not wish to be listed. (*This acknowledgement is optional.*)

- [ ] I have added the changes included in this pull request to the `CHANGELOG.md` under the next release version or unreleased, and updated the date.

- [ ] I have updated the version number in the `metadata.yaml` and config file following [semver](https://semver.org/), or the version number has already been updated. (*Leave it unchecked if you are unsure about new version number and discuss it with the infrastructure team in this PR.*)

- [ ] I have tested the pipeline on at least one A-mini sample with "run_delly = true", "run_manta = true", "run_qc = true". For run_delly = true, I have tested "variant_type" set to `gSV`, `gCNV`, and both. The paths to the test config files and output directories were attached below.

<!--- Briefly describe the changes included in this pull request and the paths to the test cases below
 !--- starting with 'Closes #...' if appropriate --->

Closes #...

**Test Results**
- Manta
	- sample:    <!-- e.g. A-mini TWGSAMIN000001-T001-S01-F, TWGSAMIN000001-T002-S02-F -->
	- input csv: <!-- /hot/pipelines/development/slurm/pipeline-call-gSV/input/call-gSV-inputs.csv -->
	- config:    <!-- /hot/pipelines/development/slurm/pipeline-call-gSV/config/nextflow-test-amini.config -->
	- output:    <!-- /hot/pipelines/development/slurm/pipeline-call-gSV/output/Manta-1.6.0 -->
- Delly - gSV
	- sample:    <!-- e.g. A-mini TWGSAMIN000001-T001-S01-F, TWGSAMIN000001-T002-S02-F -->
	- input csv: <!-- /hot/pipelines/development/slurm/pipeline-call-gSV/input/call-gSV-inputs.csv -->
	- config:    <!-- /hot/pipelines/development/slurm/pipeline-call-gSV/config/nextflow-test-amini.config -->
	- output:    <!-- /hot/pipelines/development/slurm/pipeline-call-gSV/output/Delly-0.8.7 -->
- Delly - gCNV
	- sample:    <!-- e.g. A-mini TWGSAMIN000001-T001-S01-F, TWGSAMIN000001-T002-S02-F -->
	- input csv: <!-- /hot/pipelines/development/slurm/pipeline-call-gSV/input/call-gSV-inputs.csv -->
	- config:    <!-- /hot/pipelines/development/slurm/pipeline-call-gSV/config/nextflow-test-amini.config -->
	- output:    <!-- /hot/pipelines/development/slurm/pipeline-call-gSV/output/Delly-0.8.7 --> 
- Delly - gSV & gCNV
	- sample:    <!-- e.g. A-mini TWGSAMIN000001-T001-S01-F, TWGSAMIN000001-T002-S02-F -->
	- input csv: <!-- /hot/pipelines/development/slurm/pipeline-call-gSV/input/call-gSV-inputs.csv -->
	- config:    <!-- /hot/pipelines/development/slurm/pipeline-call-gSV/config/nextflow-test-amini.config -->
	- output:    <!-- /hot/pipelines/development/slurm/pipeline-call-gSV/output/Delly-0.8.7 -->