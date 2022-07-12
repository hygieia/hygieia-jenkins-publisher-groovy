## Due to lack of activity, this repo is currently not being supported and is archived as of 07/12/22. Please note since archival, the project is not maintained and will be available in a read-only state. Please reach out to hygieia2@capitalone.com should you have any questions.
# hygieia-jenkins-publisher-groovy
groovy script alternative for Hygieia publisher plugin for Jenkins (Independent Contribution)

Issue : stageDurations object contain extra timestamps (durations) due to which the average time of stages are not correct or the value is too high.

Resolution: Added restriction to add timeInCurrentStage duration only if next stage doesn’t have any commits. Otherwise, the stage duration object will have additional values – time taken by commits to move to next stage + the age of the commit (time spent by commit in particular stage). 


The fix should resolve some open issues (closed without resolution):
Hygieia/Hygieia#1875
https://github.com/Hygieia/Hygieia/issues/2480
Hygieia/Hygieia#1298

* Added alternative feature for hygieia jenkins plugin to post deployment metrics

* Added ReadMe hygieiajenkinspluginAlt file

* Added ReadMe hygieiajenkinspluginAlt file
