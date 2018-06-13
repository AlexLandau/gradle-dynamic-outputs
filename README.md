# gradle-dynamic-outputs
Experimenting with dynamic task outputs in Gradle incremental builds

I'm looking for an approach that will allow theTask to recompute its set of output files after it runs. To see why this is important, run ./gradlew theTask --info twice, and notice that it runs twice. If you delete the generated/Monroe folder and continue running ./gradlew theTask --info, you'll see that it runs twice again before being considered up-to-date.
