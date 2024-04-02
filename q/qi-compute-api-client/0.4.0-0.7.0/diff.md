# Comparing `tmp/qi_compute_api_client-0.4.0.tar.gz` & `tmp/qi_compute_api_client-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qi_compute_api_client-0.4.0.tar", max compression
+gzip compressed data, was "qi_compute_api_client-0.7.0.tar", max compression
```

## Comparing `qi_compute_api_client-0.4.0.tar` & `qi_compute_api_client-0.7.0.tar`

### file list

```diff
@@ -1,137 +1,137 @@
--rw-r--r--   0        0        0    11357 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/LICENSE.md
--rw-r--r--   0        0        0    16473 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/README.md
--rw-r--r--   0        0        0     4692 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/__init__.py
--rw-r--r--   0        0        0     1182 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api/__init__.py
--rw-r--r--   0        0        0    31278 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api/algorithms_api.py
--rw-r--r--   0        0        0    36523 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api/batch_runs_api.py
--rw-r--r--   0        0        0    23998 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api/commits_api.py
--rw-r--r--   0        0        0    23794 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api/files_api.py
--rw-r--r--   0        0        0    19563 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api/final_results_api.py
--rw-r--r--   0        0        0    12343 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api/languages_api.py
--rw-r--r--   0        0        0    23985 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api/members_api.py
--rw-r--r--   0        0        0    19387 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api/metadata_api.py
--rw-r--r--   0        0        0    23692 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api/permissions_api.py
--rw-r--r--   0        0        0    38047 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api/projects_api.py
--rw-r--r--   0        0        0    24784 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api/reservations_api.py
--rw-r--r--   0        0        0    19106 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api/results_api.py
--rw-r--r--   0        0        0    29556 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api/runs_api.py
--rw-r--r--   0        0        0    18337 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api/runtime_api.py
--rw-r--r--   0        0        0    12235 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api/runtime_types_api.py
--rw-r--r--   0        0        0    11900 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api/teams_api.py
--rw-r--r--   0        0        0    12201 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api/transactions_api.py
--rw-r--r--   0        0        0    23783 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api/users_api.py
--rw-r--r--   0        0        0    27902 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api_client.py
--rw-r--r--   0        0        0    17035 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/configuration.py
--rw-r--r--   0        0        0      591 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/docs/Algorithm.md
--rw-r--r--   0        0        0      570 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/docs/AlgorithmIn.md
--rw-r--r--   0        0        0      308 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/docs/AlgorithmType.md
--rw-r--r--   0        0        0    14024 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/docs/AlgorithmsApi.md
--rw-r--r--   0        0        0      900 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/BatchRun.md
--rw-r--r--   0        0        0      353 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/BatchRunIn.md
--rw-r--r--   0        0        0      309 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/BatchRunStatus.md
--rw-r--r--   0        0        0    20148 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/BatchRunsApi.md
--rw-r--r--   0        0        0      445 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/Commit.md
--rw-r--r--   0        0        0      377 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/CommitIn.md
--rw-r--r--   0        0        0    11154 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/CommitsApi.md
--rw-r--r--   0        0        0      307 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/CompileStage.md
--rw-r--r--   0        0        0      301 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/Domain.md
--rw-r--r--   0        0        0      678 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/File.md
--rw-r--r--   0        0        0      668 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/FileIn.md
--rw-r--r--   0        0        0    10940 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/FilesApi.md
--rw-r--r--   0        0        0      434 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/FinalResult.md
--rw-r--r--   0        0        0      366 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/FinalResultIn.md
--rw-r--r--   0        0        0     9712 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/FinalResultsApi.md
--rw-r--r--   0        0        0      323 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/HTTPNotFoundError.md
--rw-r--r--   0        0        0      376 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/HTTPValidationError.md
--rw-r--r--   0        0        0      363 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/Language.md
--rw-r--r--   0        0        0     4893 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/LanguagesApi.md
--rw-r--r--   0        0        0      292 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/LocationInner.md
--rw-r--r--   0        0        0      498 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/Member.md
--rw-r--r--   0        0        0      477 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/MemberIn.md
--rw-r--r--   0        0        0     9315 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/MembersApi.md
--rw-r--r--   0        0        0      427 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/Metadata.md
--rw-r--r--   0        0        0     7574 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/MetadataApi.md
--rw-r--r--   0        0        0      359 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/MetadataIn.md
--rw-r--r--   0        0        0      368 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/Permission.md
--rw-r--r--   0        0        0      342 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/PermissionGroup.md
--rw-r--r--   0        0        0     9721 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/PermissionsApi.md
--rw-r--r--   0        0        0      500 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/Project.md
--rw-r--r--   0        0        0      432 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/ProjectIn.md
--rw-r--r--   0        0        0      468 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/ProjectPatch.md
--rw-r--r--   0        0        0    14529 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/ProjectsApi.md
--rw-r--r--   0        0        0      555 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/Reservation.md
--rw-r--r--   0        0        0      428 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/ReservationIn.md
--rw-r--r--   0        0        0     9962 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/ReservationsApi.md
--rw-r--r--   0        0        0      630 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/Result.md
--rw-r--r--   0        0        0      562 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/ResultIn.md
--rw-r--r--   0        0        0     9217 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/ResultsApi.md
--rw-r--r--   0        0        0      299 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/Role.md
--rw-r--r--   0        0        0      792 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/Run.md
--rw-r--r--   0        0        0      535 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/RunIn.md
--rw-r--r--   0        0        0      304 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/RunStatus.md
--rw-r--r--   0        0        0    13158 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/RunsApi.md
--rw-r--r--   0        0        0      599 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/Runtime.md
--rw-r--r--   0        0        0     7110 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/RuntimeApi.md
--rw-r--r--   0        0        0      308 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/RuntimeStatus.md
--rw-r--r--   0        0        0      617 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/RuntimeType.md
--rw-r--r--   0        0        0     4904 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/RuntimeTypesApi.md
--rw-r--r--   0        0        0      657 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/RuntimeWithAuthentication.md
--rw-r--r--   0        0        0      304 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/ShareType.md
--rw-r--r--   0        0        0      422 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/Team.md
--rw-r--r--   0        0        0     4544 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/TeamsApi.md
--rw-r--r--   0        0        0      609 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/Transaction.md
--rw-r--r--   0        0        0     4873 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/TransactionsApi.md
--rw-r--r--   0        0        0      607 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/User.md
--rw-r--r--   0        0        0      586 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/UserIn.md
--rw-r--r--   0        0        0     9119 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/UsersApi.md
--rw-r--r--   0        0        0      403 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/ValidationError.md
--rw-r--r--   0        0        0     5143 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/exceptions.py
--rw-r--r--   0        0        0     3073 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/__init__.py
--rw-r--r--   0        0        0     8684 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/algorithm.py
--rw-r--r--   0        0        0     7545 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/algorithm_in.py
--rw-r--r--   0        0        0     3195 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/algorithm_type.py
--rw-r--r--   0        0        0    14456 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/batch_run.py
--rw-r--r--   0        0        0     5910 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/batch_run_in.py
--rw-r--r--   0        0        0     3304 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/batch_run_status.py
--rw-r--r--   0        0        0     8312 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/commit.py
--rw-r--r--   0        0        0     6318 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/commit_in.py
--rw-r--r--   0        0        0     3275 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/compile_stage.py
--rw-r--r--   0        0        0     3215 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/domain.py
--rw-r--r--   0        0        0    10593 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/file.py
--rw-r--r--   0        0        0     9327 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/file_in.py
--rw-r--r--   0        0        0     7123 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/final_result.py
--rw-r--r--   0        0        0     5081 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/final_result_in.py
--rw-r--r--   0        0        0     3868 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/http_not_found_error.py
--rw-r--r--   0        0        0     3782 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/http_validation_error.py
--rw-r--r--   0        0        0     6196 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/language.py
--rw-r--r--   0        0        0     3052 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/location_inner.py
--rw-r--r--   0        0        0     8530 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/member.py
--rw-r--r--   0        0        0     7403 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/member_in.py
--rw-r--r--   0        0        0     7015 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/metadata.py
--rw-r--r--   0        0        0     4997 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/metadata_in.py
--rw-r--r--   0        0        0     6303 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/permission.py
--rw-r--r--   0        0        0     5248 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/permission_group.py
--rw-r--r--   0        0        0     8855 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/project.py
--rw-r--r--   0        0        0     6861 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/project_in.py
--rw-r--r--   0        0        0     6448 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/project_patch.py
--rw-r--r--   0        0        0    10862 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/reservation.py
--rw-r--r--   0        0        0     7732 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/reservation_in.py
--rw-r--r--   0        0        0    13635 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/result.py
--rw-r--r--   0        0        0    11673 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/result_in.py
--rw-r--r--   0        0        0     3153 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/role.py
--rw-r--r--   0        0        0    11632 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/run.py
--rw-r--r--   0        0        0     6879 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/run_in.py
--rw-r--r--   0        0        0     3290 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/run_status.py
--rw-r--r--   0        0        0     9940 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/runtime.py
--rw-r--r--   0        0        0     3273 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/runtime_status.py
--rw-r--r--   0        0        0    11585 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/runtime_type.py
--rw-r--r--   0        0        0    11844 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/runtime_with_authentication.py
--rw-r--r--   0        0        0     3212 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/share_type.py
--rw-r--r--   0        0        0     6842 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/team.py
--rw-r--r--   0        0        0    10913 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/transaction.py
--rw-r--r--   0        0        0     8950 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/user.py
--rw-r--r--   0        0        0     7847 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/user_in.py
--rw-r--r--   0        0        0     5308 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/validation_error.py
--rw-r--r--   0        0        0     9931 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/rest.py
--rw-r--r--   0        0        0     1094 2023-06-01 06:04:01.248895 qi_compute_api_client-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    17438 1970-01-01 00:00:00.000000 qi_compute_api_client-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/LICENSE.md
+-rw-r--r--   0        0        0    16473 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/README.md
+-rw-r--r--   0        0        0     4690 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/__init__.py
+-rw-r--r--   0        0        0     1182 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/api/__init__.py
+-rw-r--r--   0        0        0    31276 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/api/algorithms_api.py
+-rw-r--r--   0        0        0    36505 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/api/batch_runs_api.py
+-rw-r--r--   0        0        0    23996 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/api/commits_api.py
+-rw-r--r--   0        0        0    23792 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/api/files_api.py
+-rw-r--r--   0        0        0    19561 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/api/final_results_api.py
+-rw-r--r--   0        0        0    12341 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/api/languages_api.py
+-rw-r--r--   0        0        0    23983 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/api/members_api.py
+-rw-r--r--   0        0        0    19385 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/api/metadata_api.py
+-rw-r--r--   0        0        0    23690 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/api/permissions_api.py
+-rw-r--r--   0        0        0    38045 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/api/projects_api.py
+-rw-r--r--   0        0        0    24782 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/api/reservations_api.py
+-rw-r--r--   0        0        0    19096 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/api/results_api.py
+-rw-r--r--   0        0        0    29554 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/api/runs_api.py
+-rw-r--r--   0        0        0    18335 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/api/runtime_api.py
+-rw-r--r--   0        0        0    12233 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/api/runtime_types_api.py
+-rw-r--r--   0        0        0    11898 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/api/teams_api.py
+-rw-r--r--   0        0        0    12199 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/api/transactions_api.py
+-rw-r--r--   0        0        0    23781 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/api/users_api.py
+-rw-r--r--   0        0        0    27900 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/api_client.py
+-rw-r--r--   0        0        0    17033 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/configuration.py
+-rw-r--r--   0        0        0      591 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/Algorithm.md
+-rw-r--r--   0        0        0      570 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/AlgorithmIn.md
+-rw-r--r--   0        0        0      308 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/AlgorithmType.md
+-rw-r--r--   0        0        0    14024 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/AlgorithmsApi.md
+-rw-r--r--   0        0        0      900 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/BatchRun.md
+-rw-r--r--   0        0        0      353 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/BatchRunIn.md
+-rw-r--r--   0        0        0      309 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/BatchRunStatus.md
+-rw-r--r--   0        0        0    16463 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/BatchRunsApi.md
+-rw-r--r--   0        0        0      445 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/Commit.md
+-rw-r--r--   0        0        0      377 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/CommitIn.md
+-rw-r--r--   0        0        0    11154 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/CommitsApi.md
+-rw-r--r--   0        0        0      307 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/CompileStage.md
+-rw-r--r--   0        0        0      301 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/Domain.md
+-rw-r--r--   0        0        0      678 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/File.md
+-rw-r--r--   0        0        0      668 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/FileIn.md
+-rw-r--r--   0        0        0    10940 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/FilesApi.md
+-rw-r--r--   0        0        0      434 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/FinalResult.md
+-rw-r--r--   0        0        0      366 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/FinalResultIn.md
+-rw-r--r--   0        0        0     9712 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/FinalResultsApi.md
+-rw-r--r--   0        0        0      323 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/HTTPNotFoundError.md
+-rw-r--r--   0        0        0      376 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/HTTPValidationError.md
+-rw-r--r--   0        0        0      363 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/Language.md
+-rw-r--r--   0        0        0     4893 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/LanguagesApi.md
+-rw-r--r--   0        0        0      292 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/LocationInner.md
+-rw-r--r--   0        0        0      498 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/Member.md
+-rw-r--r--   0        0        0      477 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/MemberIn.md
+-rw-r--r--   0        0        0     9315 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/MembersApi.md
+-rw-r--r--   0        0        0      427 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/Metadata.md
+-rw-r--r--   0        0        0     7574 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/MetadataApi.md
+-rw-r--r--   0        0        0      359 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/MetadataIn.md
+-rw-r--r--   0        0        0      368 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/Permission.md
+-rw-r--r--   0        0        0      342 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/PermissionGroup.md
+-rw-r--r--   0        0        0     9721 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/PermissionsApi.md
+-rw-r--r--   0        0        0      500 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/Project.md
+-rw-r--r--   0        0        0      432 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/ProjectIn.md
+-rw-r--r--   0        0        0      468 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/ProjectPatch.md
+-rw-r--r--   0        0        0    14529 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/ProjectsApi.md
+-rw-r--r--   0        0        0      555 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/Reservation.md
+-rw-r--r--   0        0        0      428 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/ReservationIn.md
+-rw-r--r--   0        0        0     9962 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/ReservationsApi.md
+-rw-r--r--   0        0        0      630 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/Result.md
+-rw-r--r--   0        0        0      573 2023-08-02 08:33:46.042886 qi_compute_api_client-0.7.0/compute_api_client/docs/ResultIn.md
+-rw-r--r--   0        0        0     7356 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/docs/ResultsApi.md
+-rw-r--r--   0        0        0      299 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/docs/Role.md
+-rw-r--r--   0        0        0      839 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/docs/Run.md
+-rw-r--r--   0        0        0      582 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/docs/RunIn.md
+-rw-r--r--   0        0        0      304 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/docs/RunStatus.md
+-rw-r--r--   0        0        0    13158 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/docs/RunsApi.md
+-rw-r--r--   0        0        0      599 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/docs/Runtime.md
+-rw-r--r--   0        0        0     7110 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/docs/RuntimeApi.md
+-rw-r--r--   0        0        0      308 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/docs/RuntimeStatus.md
+-rw-r--r--   0        0        0      617 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/docs/RuntimeType.md
+-rw-r--r--   0        0        0     4904 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/docs/RuntimeTypesApi.md
+-rw-r--r--   0        0        0      657 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/docs/RuntimeWithAuthentication.md
+-rw-r--r--   0        0        0      304 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/docs/ShareType.md
+-rw-r--r--   0        0        0      422 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/docs/Team.md
+-rw-r--r--   0        0        0     4544 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/docs/TeamsApi.md
+-rw-r--r--   0        0        0      609 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/docs/Transaction.md
+-rw-r--r--   0        0        0     4873 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/docs/TransactionsApi.md
+-rw-r--r--   0        0        0      607 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/docs/User.md
+-rw-r--r--   0        0        0      586 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/docs/UserIn.md
+-rw-r--r--   0        0        0     9119 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/docs/UsersApi.md
+-rw-r--r--   0        0        0      403 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/docs/ValidationError.md
+-rw-r--r--   0        0        0     5141 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/exceptions.py
+-rw-r--r--   0        0        0     3071 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/__init__.py
+-rw-r--r--   0        0        0     8682 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/algorithm.py
+-rw-r--r--   0        0        0     7543 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/algorithm_in.py
+-rw-r--r--   0        0        0     3193 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/algorithm_type.py
+-rw-r--r--   0        0        0    14454 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/batch_run.py
+-rw-r--r--   0        0        0     5908 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/batch_run_in.py
+-rw-r--r--   0        0        0     3302 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/batch_run_status.py
+-rw-r--r--   0        0        0     8310 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/commit.py
+-rw-r--r--   0        0        0     6316 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/commit_in.py
+-rw-r--r--   0        0        0     3273 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/compile_stage.py
+-rw-r--r--   0        0        0     3213 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/domain.py
+-rw-r--r--   0        0        0    10591 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/file.py
+-rw-r--r--   0        0        0     9325 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/file_in.py
+-rw-r--r--   0        0        0     7121 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/final_result.py
+-rw-r--r--   0        0        0     5079 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/final_result_in.py
+-rw-r--r--   0        0        0     3866 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/http_not_found_error.py
+-rw-r--r--   0        0        0     3780 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/http_validation_error.py
+-rw-r--r--   0        0        0     6194 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/language.py
+-rw-r--r--   0        0        0     3050 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/location_inner.py
+-rw-r--r--   0        0        0     8528 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/member.py
+-rw-r--r--   0        0        0     7401 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/member_in.py
+-rw-r--r--   0        0        0     7013 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/metadata.py
+-rw-r--r--   0        0        0     4995 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/metadata_in.py
+-rw-r--r--   0        0        0     6301 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/permission.py
+-rw-r--r--   0        0        0     5246 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/permission_group.py
+-rw-r--r--   0        0        0     8853 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/project.py
+-rw-r--r--   0        0        0     6859 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/project_in.py
+-rw-r--r--   0        0        0     6446 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/project_patch.py
+-rw-r--r--   0        0        0    10860 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/reservation.py
+-rw-r--r--   0        0        0     7730 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/reservation_in.py
+-rw-r--r--   0        0        0    13633 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/result.py
+-rw-r--r--   0        0        0    11510 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/result_in.py
+-rw-r--r--   0        0        0     3151 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/role.py
+-rw-r--r--   0        0        0    12960 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/run.py
+-rw-r--r--   0        0        0     8215 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/run_in.py
+-rw-r--r--   0        0        0     3288 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/run_status.py
+-rw-r--r--   0        0        0     9938 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/runtime.py
+-rw-r--r--   0        0        0     3271 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/runtime_status.py
+-rw-r--r--   0        0        0    11583 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/runtime_type.py
+-rw-r--r--   0        0        0    11842 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/runtime_with_authentication.py
+-rw-r--r--   0        0        0     3210 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/share_type.py
+-rw-r--r--   0        0        0     6840 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/team.py
+-rw-r--r--   0        0        0    10911 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/transaction.py
+-rw-r--r--   0        0        0     8948 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/user.py
+-rw-r--r--   0        0        0     7845 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/user_in.py
+-rw-r--r--   0        0        0     5306 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/models/validation_error.py
+-rw-r--r--   0        0        0     9929 2023-08-02 08:33:46.046886 qi_compute_api_client-0.7.0/compute_api_client/rest.py
+-rw-r--r--   0        0        0     1094 2023-08-02 08:34:03.714971 qi_compute_api_client-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0    17438 1970-01-01 00:00:00.000000 qi_compute_api_client-0.7.0/PKG-INFO
```

### Comparing `qi_compute_api_client-0.4.0/LICENSE.md` & `qi_compute_api_client-0.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.4.0/README.md` & `qi_compute_api_client-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/__init__.py` & `qi_compute_api_client-0.7.0/compute_api_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 # flake8: noqa
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/api/__init__.py` & `qi_compute_api_client-0.7.0/compute_api_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/api/algorithms_api.py` & `qi_compute_api_client-0.7.0/compute_api_client/api/algorithms_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/api/batch_runs_api.py` & `qi_compute_api_client-0.7.0/compute_api_client/api/batch_runs_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
@@ -578,15 +578,15 @@
             self.api_client.select_header_content_type(
                 ['application/json'],
                 'PATCH', body_params))  # noqa: E501
         if content_types_list:
                 header_params['Content-Type'] = content_types_list
 
         # Authentication setting
-        auth_settings = ['runtime', 'user']  # noqa: E501
+        auth_settings = ['runtime']  # noqa: E501
 
         response_types_map = {
             200: "BatchRun",
             422: "HTTPValidationError",
         }
 
         return self.api_client.call_api(
@@ -706,15 +706,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['runtime', 'user']  # noqa: E501
+        auth_settings = ['runtime']  # noqa: E501
 
         response_types_map = {
             200: "BatchRun",
             404: "HTTPNotFoundError",
         }
 
         return self.api_client.call_api(
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/api/commits_api.py` & `qi_compute_api_client-0.7.0/compute_api_client/api/commits_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/api/files_api.py` & `qi_compute_api_client-0.7.0/compute_api_client/api/files_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/api/final_results_api.py` & `qi_compute_api_client-0.7.0/compute_api_client/api/final_results_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/api/languages_api.py` & `qi_compute_api_client-0.7.0/compute_api_client/api/languages_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/api/members_api.py` & `qi_compute_api_client-0.7.0/compute_api_client/api/members_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/api/metadata_api.py` & `qi_compute_api_client-0.7.0/compute_api_client/api/metadata_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/api/permissions_api.py` & `qi_compute_api_client-0.7.0/compute_api_client/api/permissions_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/api/projects_api.py` & `qi_compute_api_client-0.7.0/compute_api_client/api/projects_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/api/reservations_api.py` & `qi_compute_api_client-0.7.0/compute_api_client/api/reservations_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/api/results_api.py` & `qi_compute_api_client-0.7.0/compute_api_client/api/results_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
@@ -154,15 +154,15 @@
             self.api_client.select_header_content_type(
                 ['application/json'],
                 'POST', body_params))  # noqa: E501
         if content_types_list:
                 header_params['Content-Type'] = content_types_list
 
         # Authentication setting
-        auth_settings = ['runtime', 'user']  # noqa: E501
+        auth_settings = ['runtime']  # noqa: E501
 
         response_types_map = {
             201: "Result",
             422: "HTTPValidationError",
         }
 
         return self.api_client.call_api(
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/api/runs_api.py` & `qi_compute_api_client-0.7.0/compute_api_client/api/runs_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/api/runtime_api.py` & `qi_compute_api_client-0.7.0/compute_api_client/api/runtime_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/api/runtime_types_api.py` & `qi_compute_api_client-0.7.0/compute_api_client/api/runtime_types_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/api/teams_api.py` & `qi_compute_api_client-0.7.0/compute_api_client/api/teams_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/api/transactions_api.py` & `qi_compute_api_client-0.7.0/compute_api_client/api/transactions_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/api/users_api.py` & `qi_compute_api_client-0.7.0/compute_api_client/api/users_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/api_client.py` & `qi_compute_api_client-0.7.0/compute_api_client/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding: utf-8
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/configuration.py` & `qi_compute_api_client-0.7.0/compute_api_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/docs/Algorithm.md` & `qi_compute_api_client-0.7.0/compute_api_client/docs/Algorithm.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/docs/AlgorithmIn.md` & `qi_compute_api_client-0.7.0/compute_api_client/docs/AlgorithmIn.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/docs/AlgorithmsApi.md` & `qi_compute_api_client-0.7.0/compute_api_client/docs/AlgorithmsApi.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/docs/BatchRun.md` & `qi_compute_api_client-0.7.0/compute_api_client/docs/BatchRun.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/docs/BatchRunsApi.md` & `qi_compute_api_client-0.7.0/compute_api_client/docs/BatchRunsApi.md`

 * *Files 11% similar despite different names*

```diff
@@ -315,64 +315,14 @@
 
 # Configure API key authorization: runtime
 configuration.api_key['runtime'] = 'YOUR_API_KEY'
 
 # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
 # configuration.api_key_prefix['runtime'] = 'Bearer'
 
-# Configure API key authorization: user
-configuration.api_key['user'] = 'YOUR_API_KEY'
-
-# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
-# configuration.api_key_prefix['user'] = 'Bearer'
-
-# Enter a context with an instance of the API client
-with compute_api_client.ApiClient(configuration) as api_client:
-    # Create an instance of the API class
-    api_instance = compute_api_client.BatchRunsApi(api_client)
-    request_body = [56] # list[int] | 
-
-    try:
-        # Peek batch run
-        api_response = api_instance.peek_batch_run_batch_runs_peek_patch(request_body)
-        pprint(api_response)
-    except ApiException as e:
-        print("Exception when calling BatchRunsApi->peek_batch_run_batch_runs_peek_patch: %s\n" % e)
-```
-
-* Api Key Authentication (user):
-```python
-from __future__ import print_function
-import time
-import compute_api_client
-from compute_api_client.rest import ApiException
-from pprint import pprint
-# Defining the host is optional and defaults to http://localhost
-# See configuration.py for a list of all supported configuration parameters.
-configuration = compute_api_client.Configuration(
-    host = "http://localhost"
-)
-
-# The client must configure the authentication and authorization parameters
-# in accordance with the API server security policy.
-# Examples for each auth method are provided below, use the example that
-# satisfies your auth use case.
-
-# Configure API key authorization: runtime
-configuration.api_key['runtime'] = 'YOUR_API_KEY'
-
-# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
-# configuration.api_key_prefix['runtime'] = 'Bearer'
-
-# Configure API key authorization: user
-configuration.api_key['user'] = 'YOUR_API_KEY'
-
-# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
-# configuration.api_key_prefix['user'] = 'Bearer'
-
 # Enter a context with an instance of the API client
 with compute_api_client.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = compute_api_client.BatchRunsApi(api_client)
     request_body = [56] # list[int] | 
 
     try:
@@ -391,15 +341,15 @@
 
 ### Return type
 
 [**BatchRun**](BatchRun.md)
 
 ### Authorization
 
-[runtime](../README.md#runtime), [user](../README.md#user)
+[runtime](../README.md#runtime)
 
 ### HTTP request headers
 
  - **Content-Type**: application/json
  - **Accept**: application/json
 
 ### HTTP response details
@@ -439,63 +389,14 @@
 
 # Configure API key authorization: runtime
 configuration.api_key['runtime'] = 'YOUR_API_KEY'
 
 # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
 # configuration.api_key_prefix['runtime'] = 'Bearer'
 
-# Configure API key authorization: user
-configuration.api_key['user'] = 'YOUR_API_KEY'
-
-# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
-# configuration.api_key_prefix['user'] = 'Bearer'
-
-# Enter a context with an instance of the API client
-with compute_api_client.ApiClient(configuration) as api_client:
-    # Create an instance of the API class
-    api_instance = compute_api_client.BatchRunsApi(api_client)
-    
-    try:
-        # Take batch run
-        api_response = api_instance.pop_batch_run_batch_runs_pop_patch()
-        pprint(api_response)
-    except ApiException as e:
-        print("Exception when calling BatchRunsApi->pop_batch_run_batch_runs_pop_patch: %s\n" % e)
-```
-
-* Api Key Authentication (user):
-```python
-from __future__ import print_function
-import time
-import compute_api_client
-from compute_api_client.rest import ApiException
-from pprint import pprint
-# Defining the host is optional and defaults to http://localhost
-# See configuration.py for a list of all supported configuration parameters.
-configuration = compute_api_client.Configuration(
-    host = "http://localhost"
-)
-
-# The client must configure the authentication and authorization parameters
-# in accordance with the API server security policy.
-# Examples for each auth method are provided below, use the example that
-# satisfies your auth use case.
-
-# Configure API key authorization: runtime
-configuration.api_key['runtime'] = 'YOUR_API_KEY'
-
-# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
-# configuration.api_key_prefix['runtime'] = 'Bearer'
-
-# Configure API key authorization: user
-configuration.api_key['user'] = 'YOUR_API_KEY'
-
-# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
-# configuration.api_key_prefix['user'] = 'Bearer'
-
 # Enter a context with an instance of the API client
 with compute_api_client.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = compute_api_client.BatchRunsApi(api_client)
     
     try:
         # Take batch run
@@ -510,15 +411,15 @@
 
 ### Return type
 
 [**BatchRun**](BatchRun.md)
 
 ### Authorization
 
-[runtime](../README.md#runtime), [user](../README.md#user)
+[runtime](../README.md#runtime)
 
 ### HTTP request headers
 
  - **Content-Type**: Not defined
  - **Accept**: application/json
 
 ### HTTP response details
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/docs/CommitsApi.md` & `qi_compute_api_client-0.7.0/compute_api_client/docs/CommitsApi.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/docs/File.md` & `qi_compute_api_client-0.7.0/compute_api_client/docs/File.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/docs/FileIn.md` & `qi_compute_api_client-0.7.0/compute_api_client/docs/FileIn.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/docs/FilesApi.md` & `qi_compute_api_client-0.7.0/compute_api_client/docs/FilesApi.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/docs/FinalResultsApi.md` & `qi_compute_api_client-0.7.0/compute_api_client/docs/FinalResultsApi.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/docs/LanguagesApi.md` & `qi_compute_api_client-0.7.0/compute_api_client/docs/LanguagesApi.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/docs/MembersApi.md` & `qi_compute_api_client-0.7.0/compute_api_client/docs/MembersApi.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/docs/MetadataApi.md` & `qi_compute_api_client-0.7.0/compute_api_client/docs/MetadataApi.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/docs/PermissionsApi.md` & `qi_compute_api_client-0.7.0/compute_api_client/docs/PermissionsApi.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/docs/ProjectsApi.md` & `qi_compute_api_client-0.7.0/compute_api_client/docs/ProjectsApi.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/docs/Reservation.md` & `qi_compute_api_client-0.7.0/compute_api_client/docs/Reservation.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/docs/ReservationsApi.md` & `qi_compute_api_client-0.7.0/compute_api_client/docs/ReservationsApi.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/docs/Result.md` & `qi_compute_api_client-0.7.0/compute_api_client/docs/Result.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/docs/ResultIn.md` & `qi_compute_api_client-0.7.0/compute_api_client/docs/ResultIn.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,13 +5,13 @@
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
 **number_of_qubits** | **int** |  | 
 **execution_time_in_seconds** | **float** |  | 
 **shots_requested** | **int** |  | [optional] 
 **shots_done** | **int** |  | [optional] 
 **results** | **object** |  | [optional] 
-**metadata_id** | **int** |  | 
+**metadata_id** | **int** |  | [optional] 
 **run_id** | **int** |  | 
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/docs/ResultsApi.md` & `qi_compute_api_client-0.7.0/compute_api_client/docs/ResultsApi.md`

 * *Files 17% similar despite different names*

```diff
@@ -38,64 +38,14 @@
 
 # Configure API key authorization: runtime
 configuration.api_key['runtime'] = 'YOUR_API_KEY'
 
 # Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
 # configuration.api_key_prefix['runtime'] = 'Bearer'
 
-# Configure API key authorization: user
-configuration.api_key['user'] = 'YOUR_API_KEY'
-
-# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
-# configuration.api_key_prefix['user'] = 'Bearer'
-
-# Enter a context with an instance of the API client
-with compute_api_client.ApiClient(configuration) as api_client:
-    # Create an instance of the API class
-    api_instance = compute_api_client.ResultsApi(api_client)
-    result_in = compute_api_client.ResultIn() # ResultIn | 
-
-    try:
-        # Create result
-        api_response = api_instance.create_result_results_post(result_in)
-        pprint(api_response)
-    except ApiException as e:
-        print("Exception when calling ResultsApi->create_result_results_post: %s\n" % e)
-```
-
-* Api Key Authentication (user):
-```python
-from __future__ import print_function
-import time
-import compute_api_client
-from compute_api_client.rest import ApiException
-from pprint import pprint
-# Defining the host is optional and defaults to http://localhost
-# See configuration.py for a list of all supported configuration parameters.
-configuration = compute_api_client.Configuration(
-    host = "http://localhost"
-)
-
-# The client must configure the authentication and authorization parameters
-# in accordance with the API server security policy.
-# Examples for each auth method are provided below, use the example that
-# satisfies your auth use case.
-
-# Configure API key authorization: runtime
-configuration.api_key['runtime'] = 'YOUR_API_KEY'
-
-# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
-# configuration.api_key_prefix['runtime'] = 'Bearer'
-
-# Configure API key authorization: user
-configuration.api_key['user'] = 'YOUR_API_KEY'
-
-# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
-# configuration.api_key_prefix['user'] = 'Bearer'
-
 # Enter a context with an instance of the API client
 with compute_api_client.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = compute_api_client.ResultsApi(api_client)
     result_in = compute_api_client.ResultIn() # ResultIn | 
 
     try:
@@ -114,15 +64,15 @@
 
 ### Return type
 
 [**Result**](Result.md)
 
 ### Authorization
 
-[runtime](../README.md#runtime), [user](../README.md#user)
+[runtime](../README.md#runtime)
 
 ### HTTP request headers
 
  - **Content-Type**: application/json
  - **Accept**: application/json
 
 ### HTTP response details
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/docs/Run.md` & `qi_compute_api_client-0.7.0/compute_api_client/docs/Run.md`

 * *Files 7% similar despite different names*

```diff
@@ -6,13 +6,14 @@
 ------------ | ------------- | ------------- | -------------
 **created_on** | **datetime** |  | [readonly] 
 **queued_at** | **datetime** |  | [optional] 
 **finished_at** | **datetime** |  | [optional] 
 **id** | **int** |  | 
 **algorithm_type** | [**AlgorithmType**](AlgorithmType.md) | HYBRID: hybrid&lt;br/&gt;QUANTUM: quantum | 
 **status** | [**RunStatus**](RunStatus.md) | PLANNED: planned&lt;br/&gt;RUNNING: running&lt;br/&gt;COMPLETED: completed&lt;br/&gt;CANCELLED: cancelled&lt;br/&gt;FAILED: failed | 
+**number_of_shots** | **int** |  | [optional] 
 **batch_run_id** | **int** |  | 
 **file_id** | **int** |  | 
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/docs/RunIn.md` & `qi_compute_api_client-0.7.0/compute_api_client/docs/RunIn.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # RunIn
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
 **status** | [**RunStatus**](RunStatus.md) | PLANNED: planned&lt;br/&gt;RUNNING: running&lt;br/&gt;COMPLETED: completed&lt;br/&gt;CANCELLED: cancelled&lt;br/&gt;FAILED: failed | [optional] 
+**number_of_shots** | **int** |  | [optional] 
 **batch_run_id** | **int** |  | 
 **file_id** | **int** |  | 
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/docs/RunsApi.md` & `qi_compute_api_client-0.7.0/compute_api_client/docs/RunsApi.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/docs/Runtime.md` & `qi_compute_api_client-0.7.0/compute_api_client/docs/Runtime.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/docs/RuntimeApi.md` & `qi_compute_api_client-0.7.0/compute_api_client/docs/RuntimeApi.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/docs/RuntimeType.md` & `qi_compute_api_client-0.7.0/compute_api_client/docs/RuntimeType.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/docs/RuntimeTypesApi.md` & `qi_compute_api_client-0.7.0/compute_api_client/docs/RuntimeTypesApi.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/docs/RuntimeWithAuthentication.md` & `qi_compute_api_client-0.7.0/compute_api_client/docs/RuntimeWithAuthentication.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/docs/TeamsApi.md` & `qi_compute_api_client-0.7.0/compute_api_client/docs/TeamsApi.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/docs/Transaction.md` & `qi_compute_api_client-0.7.0/compute_api_client/docs/Transaction.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/docs/TransactionsApi.md` & `qi_compute_api_client-0.7.0/compute_api_client/docs/TransactionsApi.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/docs/User.md` & `qi_compute_api_client-0.7.0/compute_api_client/docs/User.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/docs/UserIn.md` & `qi_compute_api_client-0.7.0/compute_api_client/docs/UserIn.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/docs/UsersApi.md` & `qi_compute_api_client-0.7.0/compute_api_client/docs/UsersApi.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/exceptions.py` & `qi_compute_api_client-0.7.0/compute_api_client/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/__init__.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 # flake8: noqa
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/algorithm.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/algorithm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/algorithm_in.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/algorithm_in.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/algorithm_type.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/algorithm_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/batch_run.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/batch_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/batch_run_in.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/batch_run_in.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/batch_run_status.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/batch_run_status.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/commit.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/commit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/commit_in.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/commit_in.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/compile_stage.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/compile_stage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/domain.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/domain.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/file.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/file_in.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/file_in.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/final_result.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/final_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/final_result_in.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/final_result_in.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/http_not_found_error.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/http_not_found_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/http_validation_error.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/http_validation_error.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/language.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/language.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/location_inner.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/location_inner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/member.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/member.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/member_in.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/member_in.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/metadata.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/metadata_in.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/metadata_in.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/permission.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/permission.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/permission_group.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/permission_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/project.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/project_in.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/project_in.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/project_patch.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/project_patch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/reservation.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/reservation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/reservation_in.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/reservation_in.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/result.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/result_in.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/result_in.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
@@ -71,15 +71,16 @@
         self.discriminator = None
 
         self.number_of_qubits = number_of_qubits
         self.execution_time_in_seconds = execution_time_in_seconds
         self.shots_requested = shots_requested
         self.shots_done = shots_done
         self.results = results
-        self.metadata_id = metadata_id
+        if metadata_id is not None:
+            self.metadata_id = metadata_id
         self.run_id = run_id
 
     @property
     def number_of_qubits(self):
         """Gets the number_of_qubits of this ResultIn.  # noqa: E501
 
 
@@ -219,16 +220,14 @@
     def metadata_id(self, metadata_id):
         """Sets the metadata_id of this ResultIn.
 
 
         :param metadata_id: The metadata_id of this ResultIn.  # noqa: E501
         :type metadata_id: int
         """
-        if self.local_vars_configuration.client_side_validation and metadata_id is None:  # noqa: E501
-            raise ValueError("Invalid value for `metadata_id`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 metadata_id is not None and metadata_id > 2147483647):  # noqa: E501
             raise ValueError("Invalid value for `metadata_id`, must be a value less than or equal to `2147483647`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 metadata_id is not None and metadata_id < 1):  # noqa: E501
             raise ValueError("Invalid value for `metadata_id`, must be a value greater than or equal to `1`")  # noqa: E501
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/role.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/share_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
@@ -17,28 +17,29 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from compute_api_client.configuration import Configuration
 
 
-class Role(object):
+class ShareType(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    MEMBER = "member"
-    ADMIN = "admin"
+    PRIVATE = "private"
+    LINK_ONLY = "link_only"
+    TEAM = "team"
 
-    allowable_values = [MEMBER, ADMIN]  # noqa: E501
+    allowable_values = [PRIVATE, LINK_ONLY, TEAM]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -46,15 +47,15 @@
     openapi_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """Role - a model defined in OpenAPI"""  # noqa: E501
+        """ShareType - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
@@ -94,18 +95,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Role):
+        if not isinstance(other, ShareType):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Role):
+        if not isinstance(other, ShareType):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/run.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/run.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
@@ -38,51 +38,55 @@
     openapi_types = {
         'created_on': 'datetime',
         'queued_at': 'datetime',
         'finished_at': 'datetime',
         'id': 'int',
         'algorithm_type': 'AlgorithmType',
         'status': 'RunStatus',
+        'number_of_shots': 'int',
         'batch_run_id': 'int',
         'file_id': 'int'
     }
 
     attribute_map = {
         'created_on': 'created_on',
         'queued_at': 'queued_at',
         'finished_at': 'finished_at',
         'id': 'id',
         'algorithm_type': 'algorithm_type',
         'status': 'status',
+        'number_of_shots': 'number_of_shots',
         'batch_run_id': 'batch_run_id',
         'file_id': 'file_id'
     }
 
-    def __init__(self, created_on=None, queued_at=None, finished_at=None, id=None, algorithm_type=None, status=None, batch_run_id=None, file_id=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, created_on=None, queued_at=None, finished_at=None, id=None, algorithm_type=None, status=None, number_of_shots=None, batch_run_id=None, file_id=None, local_vars_configuration=None):  # noqa: E501
         """Run - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._created_on = None
         self._queued_at = None
         self._finished_at = None
         self._id = None
         self._algorithm_type = None
         self._status = None
+        self._number_of_shots = None
         self._batch_run_id = None
         self._file_id = None
         self.discriminator = None
 
         self.created_on = created_on
         self.queued_at = queued_at
         self.finished_at = finished_at
         self.id = id
         self.algorithm_type = algorithm_type
         self.status = status
+        self.number_of_shots = number_of_shots
         self.batch_run_id = batch_run_id
         self.file_id = file_id
 
     @property
     def created_on(self):
         """Gets the created_on of this Run.  # noqa: E501
 
@@ -229,14 +233,41 @@
         if (self.local_vars_configuration.client_side_validation and
                 status is not None and len(status) > 9):
             raise ValueError("Invalid value for `status`, length must be less than or equal to `9`")  # noqa: E501
 
         self._status = status
 
     @property
+    def number_of_shots(self):
+        """Gets the number_of_shots of this Run.  # noqa: E501
+
+
+        :return: The number_of_shots of this Run.  # noqa: E501
+        :rtype: int
+        """
+        return self._number_of_shots
+
+    @number_of_shots.setter
+    def number_of_shots(self, number_of_shots):
+        """Sets the number_of_shots of this Run.
+
+
+        :param number_of_shots: The number_of_shots of this Run.  # noqa: E501
+        :type number_of_shots: int
+        """
+        if (self.local_vars_configuration.client_side_validation and
+                number_of_shots is not None and number_of_shots > 2147483647):  # noqa: E501
+            raise ValueError("Invalid value for `number_of_shots`, must be a value less than or equal to `2147483647`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                number_of_shots is not None and number_of_shots < -2147483648):  # noqa: E501
+            raise ValueError("Invalid value for `number_of_shots`, must be a value greater than or equal to `-2147483648`")  # noqa: E501
+
+        self._number_of_shots = number_of_shots
+
+    @property
     def batch_run_id(self):
         """Gets the batch_run_id of this Run.  # noqa: E501
 
 
         :return: The batch_run_id of this Run.  # noqa: E501
         :rtype: int
         """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/run_in.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/run_in.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
@@ -33,37 +33,41 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'status': 'RunStatus',
+        'number_of_shots': 'int',
         'batch_run_id': 'int',
         'file_id': 'int'
     }
 
     attribute_map = {
         'status': 'status',
+        'number_of_shots': 'number_of_shots',
         'batch_run_id': 'batch_run_id',
         'file_id': 'file_id'
     }
 
-    def __init__(self, status=None, batch_run_id=None, file_id=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, status=None, number_of_shots=None, batch_run_id=None, file_id=None, local_vars_configuration=None):  # noqa: E501
         """RunIn - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._status = None
+        self._number_of_shots = None
         self._batch_run_id = None
         self._file_id = None
         self.discriminator = None
 
         if status is not None:
             self.status = status
+        self.number_of_shots = number_of_shots
         self.batch_run_id = batch_run_id
         self.file_id = file_id
 
     @property
     def status(self):
         """Gets the status of this RunIn.  # noqa: E501
 
@@ -86,14 +90,41 @@
         if (self.local_vars_configuration.client_side_validation and
                 status is not None and len(status) > 9):
             raise ValueError("Invalid value for `status`, length must be less than or equal to `9`")  # noqa: E501
 
         self._status = status
 
     @property
+    def number_of_shots(self):
+        """Gets the number_of_shots of this RunIn.  # noqa: E501
+
+
+        :return: The number_of_shots of this RunIn.  # noqa: E501
+        :rtype: int
+        """
+        return self._number_of_shots
+
+    @number_of_shots.setter
+    def number_of_shots(self, number_of_shots):
+        """Sets the number_of_shots of this RunIn.
+
+
+        :param number_of_shots: The number_of_shots of this RunIn.  # noqa: E501
+        :type number_of_shots: int
+        """
+        if (self.local_vars_configuration.client_side_validation and
+                number_of_shots is not None and number_of_shots > 2147483647):  # noqa: E501
+            raise ValueError("Invalid value for `number_of_shots`, must be a value less than or equal to `2147483647`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                number_of_shots is not None and number_of_shots < -2147483648):  # noqa: E501
+            raise ValueError("Invalid value for `number_of_shots`, must be a value greater than or equal to `-2147483648`")  # noqa: E501
+
+        self._number_of_shots = number_of_shots
+
+    @property
     def batch_run_id(self):
         """Gets the batch_run_id of this RunIn.  # noqa: E501
 
 
         :return: The batch_run_id of this RunIn.  # noqa: E501
         :rtype: int
         """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/run_status.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/run_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/runtime.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/runtime.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/runtime_status.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/runtime_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/runtime_type.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/runtime_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/runtime_with_authentication.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/runtime_with_authentication.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/share_type.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/role.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
@@ -17,29 +17,28 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from compute_api_client.configuration import Configuration
 
 
-class ShareType(object):
+class Role(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    PRIVATE = "private"
-    LINK_ONLY = "link_only"
-    TEAM = "team"
+    MEMBER = "member"
+    ADMIN = "admin"
 
-    allowable_values = [PRIVATE, LINK_ONLY, TEAM]  # noqa: E501
+    allowable_values = [MEMBER, ADMIN]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -47,15 +46,15 @@
     openapi_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """ShareType - a model defined in OpenAPI"""  # noqa: E501
+        """Role - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
@@ -95,18 +94,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ShareType):
+        if not isinstance(other, Role):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ShareType):
+        if not isinstance(other, Role):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/team.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/team.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/transaction.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/transaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/user.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/user_in.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/user_in.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/models/validation_error.py` & `qi_compute_api_client-0.7.0/compute_api_client/models/validation_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/compute_api_client/rest.py` & `qi_compute_api_client-0.7.0/compute_api_client/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 
 """
-    Compute Job Manager
+    Quantum Inspire 2
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `qi_compute_api_client-0.4.0/pyproject.toml` & `qi_compute_api_client-0.7.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qi-compute-api-client"
-version = "0.4.0"
+version = "0.7.0"
 description = "An API client for the Compute Job Manager of Quantum Inspire."
 license = "Apache-2.0"
 authors = ["Quantum Inspire <support@quantum-inspire.eu>"]
 readme = "README.md"
 repository = "https://github.com/QuTech-Delft/compute-api-client"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `qi_compute_api_client-0.4.0/PKG-INFO` & `qi_compute_api_client-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qi-compute-api-client
-Version: 0.4.0
+Version: 0.7.0
 Summary: An API client for the Compute Job Manager of Quantum Inspire.
 Home-page: https://github.com/QuTech-Delft/compute-api-client
 License: Apache-2.0
 Author: Quantum Inspire
 Author-email: support@quantum-inspire.eu
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
```

