# Comparing `tmp/bacalhau_apiclient-0.3.25.tar.gz` & `tmp/bacalhau_apiclient-0.3.26.tar.gz`

## Comparing `bacalhau_apiclient-0.3.25.tar` & `bacalhau_apiclient-0.3.26.tar`

### file list

```diff
@@ -1,165 +1,187 @@
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/.swagger-codegen-ignore
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/requirements.txt
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/setup.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/test-requirements.txt
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/tox.ini
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/.swagger-codegen/VERSION
--rw-r--r--   0        0        0     5898 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/__init__.py
--rw-r--r--   0        0        0    25218 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/api_client.py
--rw-r--r--   0        0        0     8164 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/configuration.py
--rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/rest.py
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/api/__init__.py
--rw-r--r--   0        0        0     6913 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/api/health_api.py
--rw-r--r--   0        0        0    29969 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/api/job_api.py
--rw-r--r--   0        0        0     5320 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/api/misc_api.py
--rw-r--r--   0        0        0    24993 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/api/utils_api.py
--rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/__init__.py
--rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/all_of_execution_state_run_output.py
--rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/all_of_execution_state_state.py
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/all_of_job_spec.py
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/all_of_job_spec_language_job_context.py
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/all_of_job_spec_wasm_entry_module.py
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/all_of_job_state_state.py
--rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/all_of_job_with_info_job.py
--rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/all_of_job_with_info_state.py
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/all_of_label_selector_requirement_operator.py
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/all_of_spec_deal.py
--rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/all_of_spec_docker.py
--rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/all_of_spec_engine.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/all_of_spec_network.py
--rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/all_of_spec_publisher.py
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/all_of_spec_resources.py
--rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/all_of_storage_spec_storage_source.py
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/all_ofcancel_request_payload.py
--rw-r--r--   0        0        0     7138 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/build_version_info.py
--rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/cancel_request.py
--rw-r--r--   0        0        0     3199 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/cancel_response.py
--rw-r--r--   0        0        0     7863 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/compute_node_info.py
--rw-r--r--   0        0        0     5955 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/deal.py
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/engine.py
--rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/events_request.py
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/events_response.py
--rw-r--r--   0        0        0    13003 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/execution_state.py
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/execution_state_type.py
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/free_space.py
--rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/health_info.py
--rw-r--r--   0        0        0     4525 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/job.py
--rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/job_cancel_payload.py
--rw-r--r--   0        0        0     8729 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/job_history.py
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/job_history_type.py
--rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/job_requester.py
--rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/job_spec_docker.py
--rw-r--r--   0        0        0     9213 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/job_spec_language.py
--rw-r--r--   0        0        0     7781 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/job_spec_wasm.py
--rw-r--r--   0        0        0     8816 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/job_state.py
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/job_state_type.py
--rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/job_with_info.py
--rw-r--r--   0        0        0     5626 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/label_selector_requirement.py
--rw-r--r--   0        0        0     7993 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/list_request.py
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/list_response.py
--rw-r--r--   0        0        0     5544 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/metadata.py
--rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/mount_status.py
--rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/network.py
--rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/network_config.py
--rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/node_info.py
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/node_type.py
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/peer_addr_info.py
--rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/published_result.py
--rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/publisher.py
--rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/resource_usage_config.py
--rw-r--r--   0        0        0     5161 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/resource_usage_data.py
--rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/results_response.py
--rw-r--r--   0        0        0     7571 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/run_command_result.py
--rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/selection_operator.py
--rw-r--r--   0        0        0    14567 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/spec.py
--rw-r--r--   0        0        0     4079 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/state_change_execution_state_type.py
--rw-r--r--   0        0        0     3971 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/state_change_job_state_type.py
--rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/state_request.py
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/state_response.py
--rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/storage_source_type.py
--rw-r--r--   0        0        0     9015 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/storage_spec.py
--rw-r--r--   0        0        0     5715 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/submit_request.py
--rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/submit_response.py
--rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/verification_result.py
--rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/verifier.py
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/version_request.py
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/version_response.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/AllOfExecutionStateRunOutput.md
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/AllOfExecutionStateState.md
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/AllOfJobSpec.md
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/AllOfJobSpecLanguageJobContext.md
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/AllOfJobSpecWasmEntryModule.md
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/AllOfJobStateState.md
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/AllOfJobWithInfoJob.md
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/AllOfJobWithInfoState.md
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/AllOfLabelSelectorRequirementOperator.md
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/AllOfSpecDeal.md
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/AllOfSpecDocker.md
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/AllOfSpecEngine.md
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/AllOfSpecNetwork.md
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/AllOfSpecPublisher.md
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/AllOfSpecResources.md
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/AllOfStorageSpecStorageSource.md
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/AllOfcancelRequestPayload.md
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/BuildVersionInfo.md
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/CancelRequest.md
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/CancelResponse.md
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/ComputeNodeInfo.md
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/Deal.md
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/Engine.md
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/EventsRequest.md
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/EventsResponse.md
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/ExecutionState.md
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/ExecutionStateType.md
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/FreeSpace.md
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/HealthApi.md
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/HealthInfo.md
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/Job.md
--rw-r--r--   0        0        0    12019 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/JobApi.md
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/JobCancelPayload.md
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/JobHistory.md
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/JobHistoryType.md
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/JobRequester.md
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/JobSpecDocker.md
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/JobSpecLanguage.md
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/JobSpecWasm.md
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/JobState.md
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/JobStateType.md
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/JobWithInfo.md
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/LabelSelectorRequirement.md
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/ListRequest.md
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/ListResponse.md
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/Metadata.md
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/MiscApi.md
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/MountStatus.md
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/Network.md
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/NetworkConfig.md
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/NodeInfo.md
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/NodeType.md
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/PeerAddrInfo.md
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/PublishedResult.md
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/Publisher.md
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/ResourceUsageConfig.md
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/ResourceUsageData.md
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/ResultsResponse.md
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/RunCommandResult.md
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/SelectionOperator.md
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/Spec.md
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/StateChangeExecutionStateType.md
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/StateChangeJobStateType.md
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/StateRequest.md
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/StateResponse.md
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/StorageSourceType.md
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/StorageSpec.md
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/SubmitRequest.md
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/SubmitResponse.md
--rw-r--r--   0        0        0     8433 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/UtilsApi.md
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/VerificationResult.md
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/Verifier.md
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/VersionRequest.md
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/docs/VersionResponse.md
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/.gitignore
--rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/LICENSE
--rw-r--r--   0        0        0     7800 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/README.md
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/pyproject.toml
--rw-r--r--   0        0        0     8374 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.25/PKG-INFO
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/.swagger-codegen-ignore
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/requirements.txt
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/setup.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/test-requirements.txt
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/tox.ini
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/.swagger-codegen/VERSION
+-rw-r--r--   0        0        0     6735 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/__init__.py
+-rw-r--r--   0        0        0    25218 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/api_client.py
+-rw-r--r--   0        0        0     8164 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/configuration.py
+-rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/rest.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/api/__init__.py
+-rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/api/default_api.py
+-rw-r--r--   0        0        0     6913 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/api/health_api.py
+-rw-r--r--   0        0        0    33905 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/api/job_api.py
+-rw-r--r--   0        0        0     5320 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/api/misc_api.py
+-rw-r--r--   0        0        0    24993 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/api/utils_api.py
+-rw-r--r--   0        0        0     6305 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/__init__.py
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/all_of_execution_state_run_output.py
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/all_of_execution_state_state.py
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/all_of_job_create_payload_spec.py
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/all_of_job_spec.py
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/all_of_job_spec_language_job_context.py
+-rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/all_of_job_spec_wasm_entry_module.py
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/all_of_job_state_state.py
+-rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/all_of_job_with_info_job.py
+-rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/all_of_job_with_info_state.py
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/all_of_label_selector_requirement_operator.py
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/all_of_spec_deal.py
+-rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/all_of_spec_docker.py
+-rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/all_of_spec_engine.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/all_of_spec_network.py
+-rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/all_of_spec_publisher.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/all_of_spec_resources.py
+-rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/all_of_storage_spec_storage_source.py
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/all_ofcancel_request_payload.py
+-rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/all_ofevents_request_filters.py
+-rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/all_oflog_request_payload.py
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/all_ofsubmit_request_payload.py
+-rw-r--r--   0        0        0     7138 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/build_version_info.py
+-rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/cancel_request.py
+-rw-r--r--   0        0        0     3199 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/cancel_response.py
+-rw-r--r--   0        0        0     7863 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/compute_node_info.py
+-rw-r--r--   0        0        0     5955 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/deal.py
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/engine.py
+-rw-r--r--   0        0        0     5064 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/event_filter_options.py
+-rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/events_request.py
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/events_response.py
+-rw-r--r--   0        0        0    14210 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/execution_state.py
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/execution_state_type.py
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/free_space.py
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/health_info.py
+-rw-r--r--   0        0        0     4525 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/job.py
+-rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/job_cancel_payload.py
+-rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/job_create_payload.py
+-rw-r--r--   0        0        0     8729 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/job_history.py
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/job_history_type.py
+-rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/job_requester.py
+-rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/job_spec_docker.py
+-rw-r--r--   0        0        0     9213 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/job_spec_language.py
+-rw-r--r--   0        0        0     7781 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/job_spec_wasm.py
+-rw-r--r--   0        0        0     8816 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/job_state.py
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/job_state_type.py
+-rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/job_with_info.py
+-rw-r--r--   0        0        0     5626 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/label_selector_requirement.py
+-rw-r--r--   0        0        0     7993 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/list_request.py
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/list_response.py
+-rw-r--r--   0        0        0     5473 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/log_request.py
+-rw-r--r--   0        0        0     6848 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/logs_payload.py
+-rw-r--r--   0        0        0     5544 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/metadata.py
+-rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/mount_status.py
+-rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/network.py
+-rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/network_config.py
+-rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/node_info.py
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/node_type.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/peer_addr_info.py
+-rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/published_result.py
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/publisher.py
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/publisher_spec.py
+-rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/resource_usage_config.py
+-rw-r--r--   0        0        0     5161 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/resource_usage_data.py
+-rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/results_response.py
+-rw-r--r--   0        0        0     7571 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/run_command_result.py
+-rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/s3_storage_spec.py
+-rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/selection_operator.py
+-rw-r--r--   0        0        0    15417 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/spec.py
+-rw-r--r--   0        0        0     4079 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/state_change_execution_state_type.py
+-rw-r--r--   0        0        0     3971 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/state_change_job_state_type.py
+-rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/state_request.py
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/state_response.py
+-rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/storage_source_type.py
+-rw-r--r--   0        0        0    10253 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/storage_spec.py
+-rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/submit_request.py
+-rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/submit_response.py
+-rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/verification_result.py
+-rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/verifier.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/version_request.py
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/version_response.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/AllOfExecutionStateRunOutput.md
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/AllOfExecutionStateState.md
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/AllOfJobCreatePayloadSpec.md
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/AllOfJobSpec.md
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/AllOfJobSpecLanguageJobContext.md
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/AllOfJobSpecWasmEntryModule.md
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/AllOfJobStateState.md
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/AllOfJobWithInfoJob.md
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/AllOfJobWithInfoState.md
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/AllOfLabelSelectorRequirementOperator.md
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/AllOfSpecDeal.md
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/AllOfSpecDocker.md
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/AllOfSpecEngine.md
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/AllOfSpecNetwork.md
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/AllOfSpecPublisher.md
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/AllOfSpecResources.md
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/AllOfStorageSpecStorageSource.md
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/AllOfcancelRequestPayload.md
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/AllOfeventsRequestFilters.md
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/AllOflogRequestPayload.md
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/AllOfsubmitRequestPayload.md
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/BuildVersionInfo.md
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/CancelRequest.md
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/CancelResponse.md
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/ComputeNodeInfo.md
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/Deal.md
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/DefaultApi.md
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/Engine.md
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/EventFilterOptions.md
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/EventsRequest.md
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/EventsResponse.md
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/ExecutionState.md
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/ExecutionStateType.md
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/FreeSpace.md
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/HealthApi.md
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/HealthInfo.md
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/Job.md
+-rw-r--r--   0        0        0    13414 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/JobApi.md
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/JobCancelPayload.md
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/JobCreatePayload.md
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/JobHistory.md
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/JobHistoryType.md
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/JobRequester.md
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/JobSpecDocker.md
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/JobSpecLanguage.md
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/JobSpecWasm.md
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/JobState.md
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/JobStateType.md
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/JobWithInfo.md
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/LabelSelectorRequirement.md
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/ListRequest.md
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/ListResponse.md
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/LogRequest.md
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/LogsPayload.md
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/Metadata.md
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/MiscApi.md
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/MountStatus.md
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/Network.md
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/NetworkConfig.md
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/NodeInfo.md
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/NodeType.md
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/PeerAddrInfo.md
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/PublishedResult.md
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/Publisher.md
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/PublisherSpec.md
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/ResourceUsageConfig.md
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/ResourceUsageData.md
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/ResultsResponse.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/RunCommandResult.md
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/S3StorageSpec.md
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/SelectionOperator.md
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/Spec.md
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/StateChangeExecutionStateType.md
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/StateChangeJobStateType.md
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/StateRequest.md
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/StateResponse.md
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/StorageSourceType.md
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/StorageSpec.md
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/SubmitRequest.md
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/SubmitResponse.md
+-rw-r--r--   0        0        0     8433 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/UtilsApi.md
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/VerificationResult.md
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/Verifier.md
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/VersionRequest.md
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/docs/VersionResponse.md
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/.gitignore
+-rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/LICENSE
+-rw-r--r--   0        0        0     8581 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/README.md
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/pyproject.toml
+-rw-r--r--   0        0        0     9155 2020-02-02 00:00:00.000000 bacalhau_apiclient-0.3.26/PKG-INFO
```

### Comparing `bacalhau_apiclient-0.3.25/.swagger-codegen-ignore` & `bacalhau_apiclient-0.3.26/.swagger-codegen-ignore`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/setup.py` & `bacalhau_apiclient-0.3.26/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Contact: team@bacalhau.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "bacalhau_apiclient"
-VERSION = "0.3.25"
+VERSION = "0.3.26"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/__init__.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 # coding: utf-8
 
 # flake8: noqa
-
 """
     Bacalhau API
 
     This page is the reference of the Bacalhau REST API. Project docs are available at https://docs.bacalhau.org/. Find more information about Bacalhau at https://github.com/bacalhau-project/bacalhau.  # noqa: E501
 
     OpenAPI spec version: ${PYPI_VERSION}
     Contact: team@bacalhau.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
-# import apis into sdk package
-from bacalhau_apiclient.api.health_api import HealthApi
-from bacalhau_apiclient.api.job_api import JobApi
-from bacalhau_apiclient.api.misc_api import MiscApi
-from bacalhau_apiclient.api.utils_api import UtilsApi
-# import ApiClient
-from bacalhau_apiclient.api_client import ApiClient
-from bacalhau_apiclient.configuration import Configuration
-# import models into sdk package
+# import models into model package
 from bacalhau_apiclient.models.all_of_execution_state_run_output import AllOfExecutionStateRunOutput
 from bacalhau_apiclient.models.all_of_execution_state_state import AllOfExecutionStateState
+from bacalhau_apiclient.models.all_of_job_create_payload_spec import AllOfJobCreatePayloadSpec
 from bacalhau_apiclient.models.all_of_job_spec import AllOfJobSpec
 from bacalhau_apiclient.models.all_of_job_spec_language_job_context import AllOfJobSpecLanguageJobContext
 from bacalhau_apiclient.models.all_of_job_spec_wasm_entry_module import AllOfJobSpecWasmEntryModule
 from bacalhau_apiclient.models.all_of_job_state_state import AllOfJobStateState
 from bacalhau_apiclient.models.all_of_job_with_info_job import AllOfJobWithInfoJob
 from bacalhau_apiclient.models.all_of_job_with_info_state import AllOfJobWithInfoState
 from bacalhau_apiclient.models.all_of_label_selector_requirement_operator import AllOfLabelSelectorRequirementOperator
@@ -36,53 +28,62 @@
 from bacalhau_apiclient.models.all_of_spec_docker import AllOfSpecDocker
 from bacalhau_apiclient.models.all_of_spec_engine import AllOfSpecEngine
 from bacalhau_apiclient.models.all_of_spec_network import AllOfSpecNetwork
 from bacalhau_apiclient.models.all_of_spec_publisher import AllOfSpecPublisher
 from bacalhau_apiclient.models.all_of_spec_resources import AllOfSpecResources
 from bacalhau_apiclient.models.all_of_storage_spec_storage_source import AllOfStorageSpecStorageSource
 from bacalhau_apiclient.models.all_ofcancel_request_payload import AllOfcancelRequestPayload
+from bacalhau_apiclient.models.all_ofevents_request_filters import AllOfeventsRequestFilters
+from bacalhau_apiclient.models.all_oflog_request_payload import AllOflogRequestPayload
+from bacalhau_apiclient.models.all_ofsubmit_request_payload import AllOfsubmitRequestPayload
 from bacalhau_apiclient.models.build_version_info import BuildVersionInfo
 from bacalhau_apiclient.models.cancel_request import CancelRequest
 from bacalhau_apiclient.models.cancel_response import CancelResponse
 from bacalhau_apiclient.models.compute_node_info import ComputeNodeInfo
 from bacalhau_apiclient.models.deal import Deal
 from bacalhau_apiclient.models.engine import Engine
+from bacalhau_apiclient.models.event_filter_options import EventFilterOptions
 from bacalhau_apiclient.models.events_request import EventsRequest
 from bacalhau_apiclient.models.events_response import EventsResponse
 from bacalhau_apiclient.models.execution_state import ExecutionState
 from bacalhau_apiclient.models.execution_state_type import ExecutionStateType
 from bacalhau_apiclient.models.free_space import FreeSpace
 from bacalhau_apiclient.models.health_info import HealthInfo
 from bacalhau_apiclient.models.job import Job
 from bacalhau_apiclient.models.job_cancel_payload import JobCancelPayload
+from bacalhau_apiclient.models.job_create_payload import JobCreatePayload
 from bacalhau_apiclient.models.job_history import JobHistory
 from bacalhau_apiclient.models.job_history_type import JobHistoryType
 from bacalhau_apiclient.models.job_requester import JobRequester
 from bacalhau_apiclient.models.job_spec_docker import JobSpecDocker
 from bacalhau_apiclient.models.job_spec_language import JobSpecLanguage
 from bacalhau_apiclient.models.job_spec_wasm import JobSpecWasm
 from bacalhau_apiclient.models.job_state import JobState
 from bacalhau_apiclient.models.job_state_type import JobStateType
 from bacalhau_apiclient.models.job_with_info import JobWithInfo
 from bacalhau_apiclient.models.label_selector_requirement import LabelSelectorRequirement
 from bacalhau_apiclient.models.list_request import ListRequest
 from bacalhau_apiclient.models.list_response import ListResponse
+from bacalhau_apiclient.models.log_request import LogRequest
+from bacalhau_apiclient.models.logs_payload import LogsPayload
 from bacalhau_apiclient.models.metadata import Metadata
 from bacalhau_apiclient.models.mount_status import MountStatus
 from bacalhau_apiclient.models.network import Network
 from bacalhau_apiclient.models.network_config import NetworkConfig
 from bacalhau_apiclient.models.node_info import NodeInfo
 from bacalhau_apiclient.models.node_type import NodeType
 from bacalhau_apiclient.models.peer_addr_info import PeerAddrInfo
 from bacalhau_apiclient.models.published_result import PublishedResult
 from bacalhau_apiclient.models.publisher import Publisher
+from bacalhau_apiclient.models.publisher_spec import PublisherSpec
 from bacalhau_apiclient.models.resource_usage_config import ResourceUsageConfig
 from bacalhau_apiclient.models.resource_usage_data import ResourceUsageData
 from bacalhau_apiclient.models.results_response import ResultsResponse
 from bacalhau_apiclient.models.run_command_result import RunCommandResult
+from bacalhau_apiclient.models.s3_storage_spec import S3StorageSpec
 from bacalhau_apiclient.models.selection_operator import SelectionOperator
 from bacalhau_apiclient.models.spec import Spec
 from bacalhau_apiclient.models.state_change_execution_state_type import StateChangeExecutionStateType
 from bacalhau_apiclient.models.state_change_job_state_type import StateChangeJobStateType
 from bacalhau_apiclient.models.state_request import StateRequest
 from bacalhau_apiclient.models.state_response import StateResponse
 from bacalhau_apiclient.models.storage_source_type import StorageSourceType
```

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/api_client.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         self.pool = ThreadPool()
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/0.3.25/python'
+        self.user_agent = 'Swagger-Codegen/0.3.26/python'
 
     def __del__(self):
         self.pool.close()
         self.pool.join()
 
     @property
     def user_agent(self):
```

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/configuration.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,9 +236,9 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: ${PYPI_VERSION}\n"\
-               "SDK Package Version: 0.3.25".\
+               "SDK Package Version: 0.3.26".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/rest.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/rest.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/api/health_api.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/api/health_api.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/api/job_api.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/api/job_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -325,14 +325,113 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def logs(self, body, **kwargs):  # noqa: E501
+        """Displays the logs for a current job/execution  # noqa: E501
+
+        Shows the output from the job specified by `id` as long as that job belongs to `client_id`.  The ouput will be continuous until either, the client disconnects or the execution completes.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.logs(body, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param LogRequest body: (required)
+        :return: str
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.logs_with_http_info(body, **kwargs)  # noqa: E501
+        else:
+            (data) = self.logs_with_http_info(body, **kwargs)  # noqa: E501
+            return data
+
+    def logs_with_http_info(self, body, **kwargs):  # noqa: E501
+        """Displays the logs for a current job/execution  # noqa: E501
+
+        Shows the output from the job specified by `id` as long as that job belongs to `client_id`.  The ouput will be continuous until either, the client disconnects or the execution completes.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.logs_with_http_info(body, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param LogRequest body: (required)
+        :return: str
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['body']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method logs" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'body' is set
+        if ('body' not in params or
+                params['body'] is None):
+            raise ValueError("Missing the required parameter `body` when calling `logs`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'body' in params:
+            body_params = params['body']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = []  # noqa: E501
+
+        return self.api_client.call_api(
+            '/requester/logs', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='str',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def results(self, body, **kwargs):  # noqa: E501
         """Returns the results of the job-id specified in the body payload.  # noqa: E501
 
         Example response:  ```json {   \"results\": [     {       \"NodeID\": \"QmdZQ7ZbhnvWY1J12XYKGHApJ6aufKyLNSvf8jZBrBaAVL\",       \"Data\": {         \"StorageSource\": \"IPFS\",         \"Name\": \"job-9304c616-291f-41ad-b862-54e133c0149e-shard-0-host-QmdZQ7ZbhnvWY1J12XYKGHApJ6aufKyLNSvf8jZBrBaAVL\",         \"CID\": \"QmTVmC7JBD2ES2qGPqBNVWnX1KeEPNrPGb7rJ8cpFgtefe\"       }     }   ] } ```  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.results(body, async_req=True)
@@ -526,15 +625,15 @@
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def submit(self, body, **kwargs):  # noqa: E501
         """Submits a new job to the network.  # noqa: E501
 
-        Description:  * `client_public_key`: The base64-encoded public key of the client. * `signature`: A base64-encoded signature of the `data` attribute, signed by the client. * `job_create_payload`:     * `ClientID`: Request must specify a `ClientID`. To retrieve your `ClientID`, you can do the following: (1) submit a dummy job to Bacalhau (or use one you created before), (2) run `bacalhau describe <job-id>` and fetch the `ClientID` field.  * `APIVersion`: e.g. `\"V1beta1\"`.     * `Spec`: https://github.com/bacalhau-project/bacalhau/blob/main/pkg/job.go   # noqa: E501
+        Description:  * `client_public_key`: The base64-encoded public key of the client. * `signature`: A base64-encoded signature of the `data` attribute, signed by the client. * `payload`:     * `ClientID`: Request must specify a `ClientID`. To retrieve your `ClientID`, you can do the following: (1) submit a dummy job to Bacalhau (or use one you created before), (2) run `bacalhau describe <job-id>` and fetch the `ClientID` field.  * `APIVersion`: e.g. `\"V1beta1\"`.     * `Spec`: https://github.com/bacalhau-project/bacalhau/blob/main/pkg/job.go   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.submit(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param SubmitRequest body: (required)
@@ -548,15 +647,15 @@
         else:
             (data) = self.submit_with_http_info(body, **kwargs)  # noqa: E501
             return data
 
     def submit_with_http_info(self, body, **kwargs):  # noqa: E501
         """Submits a new job to the network.  # noqa: E501
 
-        Description:  * `client_public_key`: The base64-encoded public key of the client. * `signature`: A base64-encoded signature of the `data` attribute, signed by the client. * `job_create_payload`:     * `ClientID`: Request must specify a `ClientID`. To retrieve your `ClientID`, you can do the following: (1) submit a dummy job to Bacalhau (or use one you created before), (2) run `bacalhau describe <job-id>` and fetch the `ClientID` field.  * `APIVersion`: e.g. `\"V1beta1\"`.     * `Spec`: https://github.com/bacalhau-project/bacalhau/blob/main/pkg/job.go   # noqa: E501
+        Description:  * `client_public_key`: The base64-encoded public key of the client. * `signature`: A base64-encoded signature of the `data` attribute, signed by the client. * `payload`:     * `ClientID`: Request must specify a `ClientID`. To retrieve your `ClientID`, you can do the following: (1) submit a dummy job to Bacalhau (or use one you created before), (2) run `bacalhau describe <job-id>` and fetch the `ClientID` field.  * `APIVersion`: e.g. `\"V1beta1\"`.     * `Spec`: https://github.com/bacalhau-project/bacalhau/blob/main/pkg/job.go   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.submit_with_http_info(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param SubmitRequest body: (required)
```

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/api/misc_api.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/api/misc_api.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/api/utils_api.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/api/utils_api.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/__init__.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,36 @@
 # coding: utf-8
 
 # flake8: noqa
+
 """
     Bacalhau API
 
     This page is the reference of the Bacalhau REST API. Project docs are available at https://docs.bacalhau.org/. Find more information about Bacalhau at https://github.com/bacalhau-project/bacalhau.  # noqa: E501
 
     OpenAPI spec version: ${PYPI_VERSION}
     Contact: team@bacalhau.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
-# import models into model package
+# import apis into sdk package
+from bacalhau_apiclient.api.health_api import HealthApi
+from bacalhau_apiclient.api.job_api import JobApi
+from bacalhau_apiclient.api.misc_api import MiscApi
+from bacalhau_apiclient.api.utils_api import UtilsApi
+from bacalhau_apiclient.api.default_api import DefaultApi
+# import ApiClient
+from bacalhau_apiclient.api_client import ApiClient
+from bacalhau_apiclient.configuration import Configuration
+# import models into sdk package
 from bacalhau_apiclient.models.all_of_execution_state_run_output import AllOfExecutionStateRunOutput
 from bacalhau_apiclient.models.all_of_execution_state_state import AllOfExecutionStateState
+from bacalhau_apiclient.models.all_of_job_create_payload_spec import AllOfJobCreatePayloadSpec
 from bacalhau_apiclient.models.all_of_job_spec import AllOfJobSpec
 from bacalhau_apiclient.models.all_of_job_spec_language_job_context import AllOfJobSpecLanguageJobContext
 from bacalhau_apiclient.models.all_of_job_spec_wasm_entry_module import AllOfJobSpecWasmEntryModule
 from bacalhau_apiclient.models.all_of_job_state_state import AllOfJobStateState
 from bacalhau_apiclient.models.all_of_job_with_info_job import AllOfJobWithInfoJob
 from bacalhau_apiclient.models.all_of_job_with_info_state import AllOfJobWithInfoState
 from bacalhau_apiclient.models.all_of_label_selector_requirement_operator import AllOfLabelSelectorRequirementOperator
@@ -27,53 +38,62 @@
 from bacalhau_apiclient.models.all_of_spec_docker import AllOfSpecDocker
 from bacalhau_apiclient.models.all_of_spec_engine import AllOfSpecEngine
 from bacalhau_apiclient.models.all_of_spec_network import AllOfSpecNetwork
 from bacalhau_apiclient.models.all_of_spec_publisher import AllOfSpecPublisher
 from bacalhau_apiclient.models.all_of_spec_resources import AllOfSpecResources
 from bacalhau_apiclient.models.all_of_storage_spec_storage_source import AllOfStorageSpecStorageSource
 from bacalhau_apiclient.models.all_ofcancel_request_payload import AllOfcancelRequestPayload
+from bacalhau_apiclient.models.all_ofevents_request_filters import AllOfeventsRequestFilters
+from bacalhau_apiclient.models.all_oflog_request_payload import AllOflogRequestPayload
+from bacalhau_apiclient.models.all_ofsubmit_request_payload import AllOfsubmitRequestPayload
 from bacalhau_apiclient.models.build_version_info import BuildVersionInfo
 from bacalhau_apiclient.models.cancel_request import CancelRequest
 from bacalhau_apiclient.models.cancel_response import CancelResponse
 from bacalhau_apiclient.models.compute_node_info import ComputeNodeInfo
 from bacalhau_apiclient.models.deal import Deal
 from bacalhau_apiclient.models.engine import Engine
+from bacalhau_apiclient.models.event_filter_options import EventFilterOptions
 from bacalhau_apiclient.models.events_request import EventsRequest
 from bacalhau_apiclient.models.events_response import EventsResponse
 from bacalhau_apiclient.models.execution_state import ExecutionState
 from bacalhau_apiclient.models.execution_state_type import ExecutionStateType
 from bacalhau_apiclient.models.free_space import FreeSpace
 from bacalhau_apiclient.models.health_info import HealthInfo
 from bacalhau_apiclient.models.job import Job
 from bacalhau_apiclient.models.job_cancel_payload import JobCancelPayload
+from bacalhau_apiclient.models.job_create_payload import JobCreatePayload
 from bacalhau_apiclient.models.job_history import JobHistory
 from bacalhau_apiclient.models.job_history_type import JobHistoryType
 from bacalhau_apiclient.models.job_requester import JobRequester
 from bacalhau_apiclient.models.job_spec_docker import JobSpecDocker
 from bacalhau_apiclient.models.job_spec_language import JobSpecLanguage
 from bacalhau_apiclient.models.job_spec_wasm import JobSpecWasm
 from bacalhau_apiclient.models.job_state import JobState
 from bacalhau_apiclient.models.job_state_type import JobStateType
 from bacalhau_apiclient.models.job_with_info import JobWithInfo
 from bacalhau_apiclient.models.label_selector_requirement import LabelSelectorRequirement
 from bacalhau_apiclient.models.list_request import ListRequest
 from bacalhau_apiclient.models.list_response import ListResponse
+from bacalhau_apiclient.models.log_request import LogRequest
+from bacalhau_apiclient.models.logs_payload import LogsPayload
 from bacalhau_apiclient.models.metadata import Metadata
 from bacalhau_apiclient.models.mount_status import MountStatus
 from bacalhau_apiclient.models.network import Network
 from bacalhau_apiclient.models.network_config import NetworkConfig
 from bacalhau_apiclient.models.node_info import NodeInfo
 from bacalhau_apiclient.models.node_type import NodeType
 from bacalhau_apiclient.models.peer_addr_info import PeerAddrInfo
 from bacalhau_apiclient.models.published_result import PublishedResult
 from bacalhau_apiclient.models.publisher import Publisher
+from bacalhau_apiclient.models.publisher_spec import PublisherSpec
 from bacalhau_apiclient.models.resource_usage_config import ResourceUsageConfig
 from bacalhau_apiclient.models.resource_usage_data import ResourceUsageData
 from bacalhau_apiclient.models.results_response import ResultsResponse
 from bacalhau_apiclient.models.run_command_result import RunCommandResult
+from bacalhau_apiclient.models.s3_storage_spec import S3StorageSpec
 from bacalhau_apiclient.models.selection_operator import SelectionOperator
 from bacalhau_apiclient.models.spec import Spec
 from bacalhau_apiclient.models.state_change_execution_state_type import StateChangeExecutionStateType
 from bacalhau_apiclient.models.state_change_job_state_type import StateChangeJobStateType
 from bacalhau_apiclient.models.state_request import StateRequest
 from bacalhau_apiclient.models.state_response import StateResponse
 from bacalhau_apiclient.models.storage_source_type import StorageSourceType
```

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/all_of_execution_state_run_output.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/all_of_execution_state_run_output.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/all_of_execution_state_state.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/all_of_execution_state_state.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/all_of_job_spec.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/all_of_job_spec.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/all_of_job_spec_language_job_context.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/all_of_job_spec_language_job_context.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/all_of_job_spec_wasm_entry_module.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/all_of_job_spec_wasm_entry_module.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/all_of_job_state_state.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/all_of_job_state_state.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/all_of_job_with_info_job.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/all_of_job_with_info_job.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/all_of_job_with_info_state.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/all_of_job_with_info_state.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/all_of_label_selector_requirement_operator.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/all_of_label_selector_requirement_operator.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/all_of_spec_deal.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/all_of_spec_deal.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/all_of_spec_docker.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/all_of_spec_docker.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/all_of_spec_engine.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/all_of_spec_engine.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/all_of_spec_network.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/all_of_spec_network.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/all_of_spec_publisher.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/all_of_spec_publisher.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/all_of_spec_resources.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/all_of_spec_resources.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/all_of_storage_spec_storage_source.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/all_of_storage_spec_storage_source.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/all_ofcancel_request_payload.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/all_ofcancel_request_payload.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/build_version_info.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/build_version_info.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/cancel_request.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/cancel_request.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/cancel_response.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/cancel_response.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/compute_node_info.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/compute_node_info.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/deal.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/deal.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/engine.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/engine.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/events_request.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/state_request.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class EventsRequest(object):
+class StateRequest(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -34,60 +34,60 @@
 
     attribute_map = {
         'client_id': 'client_id',
         'job_id': 'job_id'
     }
 
     def __init__(self, client_id=None, job_id=None):  # noqa: E501
-        """EventsRequest - a model defined in Swagger"""  # noqa: E501
+        """StateRequest - a model defined in Swagger"""  # noqa: E501
         self._client_id = None
         self._job_id = None
         self.discriminator = None
         if client_id is not None:
             self.client_id = client_id
         if job_id is not None:
             self.job_id = job_id
 
     @property
     def client_id(self):
-        """Gets the client_id of this EventsRequest.  # noqa: E501
+        """Gets the client_id of this StateRequest.  # noqa: E501
 
 
-        :return: The client_id of this EventsRequest.  # noqa: E501
+        :return: The client_id of this StateRequest.  # noqa: E501
         :rtype: str
         """
         return self._client_id
 
     @client_id.setter
     def client_id(self, client_id):
-        """Sets the client_id of this EventsRequest.
+        """Sets the client_id of this StateRequest.
 
 
-        :param client_id: The client_id of this EventsRequest.  # noqa: E501
+        :param client_id: The client_id of this StateRequest.  # noqa: E501
         :type: str
         """
 
         self._client_id = client_id
 
     @property
     def job_id(self):
-        """Gets the job_id of this EventsRequest.  # noqa: E501
+        """Gets the job_id of this StateRequest.  # noqa: E501
 
 
-        :return: The job_id of this EventsRequest.  # noqa: E501
+        :return: The job_id of this StateRequest.  # noqa: E501
         :rtype: str
         """
         return self._job_id
 
     @job_id.setter
     def job_id(self, job_id):
-        """Sets the job_id of this EventsRequest.
+        """Sets the job_id of this StateRequest.
 
 
-        :param job_id: The job_id of this EventsRequest.  # noqa: E501
+        :param job_id: The job_id of this StateRequest.  # noqa: E501
         :type: str
         """
 
         self._job_id = job_id
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -106,15 +106,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(EventsRequest, dict):
+        if issubclass(StateRequest, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,15 +122,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, EventsRequest):
+        if not isinstance(other, StateRequest):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/events_response.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/events_response.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/execution_state.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/execution_state.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
+        'accepted_ask_for_bid': 'bool',
         'compute_reference': 'str',
         'create_time': 'str',
         'job_id': 'str',
         'node_id': 'str',
         'published_results': 'StorageSpec',
         'run_output': 'AllOfExecutionStateRunOutput',
         'state': 'AllOfExecutionStateState',
@@ -39,43 +40,47 @@
         'update_time': 'str',
         'verification_proposal': 'list[int]',
         'verification_result': 'VerificationResult',
         'version': 'int'
     }
 
     attribute_map = {
+        'accepted_ask_for_bid': 'AcceptedAskForBid',
         'compute_reference': 'ComputeReference',
         'create_time': 'CreateTime',
         'job_id': 'JobID',
         'node_id': 'NodeId',
         'published_results': 'PublishedResults',
         'run_output': 'RunOutput',
         'state': 'State',
         'status': 'Status',
         'update_time': 'UpdateTime',
         'verification_proposal': 'VerificationProposal',
         'verification_result': 'VerificationResult',
         'version': 'Version'
     }
 
-    def __init__(self, compute_reference=None, create_time=None, job_id=None, node_id=None, published_results=None, run_output=None, state=None, status=None, update_time=None, verification_proposal=None, verification_result=None, version=None):  # noqa: E501
+    def __init__(self, accepted_ask_for_bid=None, compute_reference=None, create_time=None, job_id=None, node_id=None, published_results=None, run_output=None, state=None, status=None, update_time=None, verification_proposal=None, verification_result=None, version=None):  # noqa: E501
         """ExecutionState - a model defined in Swagger"""  # noqa: E501
+        self._accepted_ask_for_bid = None
         self._compute_reference = None
         self._create_time = None
         self._job_id = None
         self._node_id = None
         self._published_results = None
         self._run_output = None
         self._state = None
         self._status = None
         self._update_time = None
         self._verification_proposal = None
         self._verification_result = None
         self._version = None
         self.discriminator = None
+        if accepted_ask_for_bid is not None:
+            self.accepted_ask_for_bid = accepted_ask_for_bid
         if compute_reference is not None:
             self.compute_reference = compute_reference
         if create_time is not None:
             self.create_time = create_time
         if job_id is not None:
             self.job_id = job_id
         if node_id is not None:
@@ -94,14 +99,37 @@
             self.verification_proposal = verification_proposal
         if verification_result is not None:
             self.verification_result = verification_result
         if version is not None:
             self.version = version
 
     @property
+    def accepted_ask_for_bid(self):
+        """Gets the accepted_ask_for_bid of this ExecutionState.  # noqa: E501
+
+        Set to true iff the compute node accepted the ask for a bid, and intends to run the job if the bid is accepted by the requester.  # noqa: E501
+
+        :return: The accepted_ask_for_bid of this ExecutionState.  # noqa: E501
+        :rtype: bool
+        """
+        return self._accepted_ask_for_bid
+
+    @accepted_ask_for_bid.setter
+    def accepted_ask_for_bid(self, accepted_ask_for_bid):
+        """Sets the accepted_ask_for_bid of this ExecutionState.
+
+        Set to true iff the compute node accepted the ask for a bid, and intends to run the job if the bid is accepted by the requester.  # noqa: E501
+
+        :param accepted_ask_for_bid: The accepted_ask_for_bid of this ExecutionState.  # noqa: E501
+        :type: bool
+        """
+
+        self._accepted_ask_for_bid = accepted_ask_for_bid
+
+    @property
     def compute_reference(self):
         """Gets the compute_reference of this ExecutionState.  # noqa: E501
 
         Compute node reference for this job execution  # noqa: E501
 
         :return: The compute_reference of this ExecutionState.  # noqa: E501
         :rtype: str
```

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/execution_state_type.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/execution_state_type.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/free_space.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/free_space.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/health_info.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/health_info.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/job.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/job.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/job_cancel_payload.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/job_cancel_payload.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/job_history.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/job_history.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/job_history_type.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/job_history_type.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/job_requester.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/job_requester.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/job_spec_docker.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/job_spec_docker.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/job_spec_language.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/job_spec_language.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/job_spec_wasm.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/job_spec_wasm.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/job_state.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/job_state.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/job_state_type.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/job_state_type.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/job_with_info.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/job_with_info.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/label_selector_requirement.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/label_selector_requirement.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/list_request.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/list_request.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/list_response.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/list_response.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/metadata.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/metadata.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/mount_status.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/mount_status.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/network.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/network.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/network_config.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/network_config.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/node_info.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/node_info.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/node_type.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/node_type.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/peer_addr_info.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/peer_addr_info.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/published_result.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/published_result.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/publisher.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/publisher.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     """
     _0 = "0"
     _1 = "1"
     _2 = "2"
     _3 = "3"
     _4 = "4"
     _5 = "5"
+    _6 = "6"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/resource_usage_config.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/resource_usage_config.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/resource_usage_data.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/resource_usage_data.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/results_response.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/results_response.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/run_command_result.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/run_command_result.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/selection_operator.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/selection_operator.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/spec.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/spec.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         'do_not_track': 'bool',
         'docker': 'AllOfSpecDocker',
         'engine': 'AllOfSpecEngine',
         'language': 'JobSpecLanguage',
         'network': 'AllOfSpecNetwork',
         'node_selectors': 'list[LabelSelectorRequirement]',
         'publisher': 'AllOfSpecPublisher',
+        'publisher_spec': 'PublisherSpec',
         'resources': 'AllOfSpecResources',
         'timeout': 'float',
         'verifier': 'Verifier',
         'wasm': 'JobSpecWasm',
         'inputs': 'list[StorageSpec]',
         'outputs': 'list[StorageSpec]'
     }
@@ -51,33 +52,35 @@
         'do_not_track': 'DoNotTrack',
         'docker': 'Docker',
         'engine': 'Engine',
         'language': 'Language',
         'network': 'Network',
         'node_selectors': 'NodeSelectors',
         'publisher': 'Publisher',
+        'publisher_spec': 'PublisherSpec',
         'resources': 'Resources',
         'timeout': 'Timeout',
         'verifier': 'Verifier',
         'wasm': 'Wasm',
         'inputs': 'inputs',
         'outputs': 'outputs'
     }
 
-    def __init__(self, annotations=None, deal=None, do_not_track=None, docker=None, engine=None, language=None, network=None, node_selectors=None, publisher=None, resources=None, timeout=None, verifier=None, wasm=None, inputs=None, outputs=None):  # noqa: E501
+    def __init__(self, annotations=None, deal=None, do_not_track=None, docker=None, engine=None, language=None, network=None, node_selectors=None, publisher=None, publisher_spec=None, resources=None, timeout=None, verifier=None, wasm=None, inputs=None, outputs=None):  # noqa: E501
         """Spec - a model defined in Swagger"""  # noqa: E501
         self._annotations = None
         self._deal = None
         self._do_not_track = None
         self._docker = None
         self._engine = None
         self._language = None
         self._network = None
         self._node_selectors = None
         self._publisher = None
+        self._publisher_spec = None
         self._resources = None
         self._timeout = None
         self._verifier = None
         self._wasm = None
         self._inputs = None
         self._outputs = None
         self.discriminator = None
@@ -95,14 +98,16 @@
             self.language = language
         if network is not None:
             self.network = network
         if node_selectors is not None:
             self.node_selectors = node_selectors
         if publisher is not None:
             self.publisher = publisher
+        if publisher_spec is not None:
+            self.publisher_spec = publisher_spec
         if resources is not None:
             self.resources = resources
         if timeout is not None:
             self.timeout = timeout
         if verifier is not None:
             self.verifier = verifier
         if wasm is not None:
@@ -294,34 +299,55 @@
 
         self._node_selectors = node_selectors
 
     @property
     def publisher(self):
         """Gets the publisher of this Spec.  # noqa: E501
 
-        there can be multiple publishers for the job  # noqa: E501
+        there can be multiple publishers for the job deprecated: use PublisherSpec instead  # noqa: E501
 
         :return: The publisher of this Spec.  # noqa: E501
         :rtype: AllOfSpecPublisher
         """
         return self._publisher
 
     @publisher.setter
     def publisher(self, publisher):
         """Sets the publisher of this Spec.
 
-        there can be multiple publishers for the job  # noqa: E501
+        there can be multiple publishers for the job deprecated: use PublisherSpec instead  # noqa: E501
 
         :param publisher: The publisher of this Spec.  # noqa: E501
         :type: AllOfSpecPublisher
         """
 
         self._publisher = publisher
 
     @property
+    def publisher_spec(self):
+        """Gets the publisher_spec of this Spec.  # noqa: E501
+
+
+        :return: The publisher_spec of this Spec.  # noqa: E501
+        :rtype: PublisherSpec
+        """
+        return self._publisher_spec
+
+    @publisher_spec.setter
+    def publisher_spec(self, publisher_spec):
+        """Sets the publisher_spec of this Spec.
+
+
+        :param publisher_spec: The publisher_spec of this Spec.  # noqa: E501
+        :type: PublisherSpec
+        """
+
+        self._publisher_spec = publisher_spec
+
+    @property
     def resources(self):
         """Gets the resources of this Spec.  # noqa: E501
 
         the compute (cpu, ram) resources this job requires  # noqa: E501
 
         :return: The resources of this Spec.  # noqa: E501
         :rtype: AllOfSpecResources
```

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/state_change_execution_state_type.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/state_change_execution_state_type.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/state_change_job_state_type.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/state_change_job_state_type.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/state_request.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/version_request.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,88 +11,62 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class StateRequest(object):
+class VersionRequest(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'client_id': 'str',
-        'job_id': 'str'
+        'client_id': 'str'
     }
 
     attribute_map = {
-        'client_id': 'client_id',
-        'job_id': 'job_id'
+        'client_id': 'client_id'
     }
 
-    def __init__(self, client_id=None, job_id=None):  # noqa: E501
-        """StateRequest - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, client_id=None):  # noqa: E501
+        """VersionRequest - a model defined in Swagger"""  # noqa: E501
         self._client_id = None
-        self._job_id = None
         self.discriminator = None
         if client_id is not None:
             self.client_id = client_id
-        if job_id is not None:
-            self.job_id = job_id
 
     @property
     def client_id(self):
-        """Gets the client_id of this StateRequest.  # noqa: E501
+        """Gets the client_id of this VersionRequest.  # noqa: E501
 
 
-        :return: The client_id of this StateRequest.  # noqa: E501
+        :return: The client_id of this VersionRequest.  # noqa: E501
         :rtype: str
         """
         return self._client_id
 
     @client_id.setter
     def client_id(self, client_id):
-        """Sets the client_id of this StateRequest.
+        """Sets the client_id of this VersionRequest.
 
 
-        :param client_id: The client_id of this StateRequest.  # noqa: E501
+        :param client_id: The client_id of this VersionRequest.  # noqa: E501
         :type: str
         """
 
         self._client_id = client_id
 
-    @property
-    def job_id(self):
-        """Gets the job_id of this StateRequest.  # noqa: E501
-
-
-        :return: The job_id of this StateRequest.  # noqa: E501
-        :rtype: str
-        """
-        return self._job_id
-
-    @job_id.setter
-    def job_id(self, job_id):
-        """Sets the job_id of this StateRequest.
-
-
-        :param job_id: The job_id of this StateRequest.  # noqa: E501
-        :type: str
-        """
-
-        self._job_id = job_id
-
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -106,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(StateRequest, dict):
+        if issubclass(VersionRequest, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, StateRequest):
+        if not isinstance(other, VersionRequest):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/state_response.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/state_response.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/storage_source_type.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/storage_source_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,17 @@
     _2 = "2"
     _3 = "3"
     _4 = "4"
     _5 = "5"
     _6 = "6"
     _7 = "7"
     _8 = "8"
+    _9 = "9"
+    _10 = "10"
+    _11 = "11"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/storage_spec.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/storage_spec.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,46 +27,56 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'cid': 'str',
         'metadata': 'dict(str, str)',
         'name': 'str',
+        'repo': 'str',
+        's3': 'S3StorageSpec',
         'source_path': 'str',
         'storage_source': 'AllOfStorageSpecStorageSource',
         'url': 'str',
         'path': 'str'
     }
 
     attribute_map = {
         'cid': 'CID',
         'metadata': 'Metadata',
         'name': 'Name',
+        'repo': 'Repo',
+        's3': 'S3',
         'source_path': 'SourcePath',
         'storage_source': 'StorageSource',
         'url': 'URL',
         'path': 'path'
     }
 
-    def __init__(self, cid=None, metadata=None, name=None, source_path=None, storage_source=None, url=None, path=None):  # noqa: E501
+    def __init__(self, cid=None, metadata=None, name=None, repo=None, s3=None, source_path=None, storage_source=None, url=None, path=None):  # noqa: E501
         """StorageSpec - a model defined in Swagger"""  # noqa: E501
         self._cid = None
         self._metadata = None
         self._name = None
+        self._repo = None
+        self._s3 = None
         self._source_path = None
         self._storage_source = None
         self._url = None
         self._path = None
         self.discriminator = None
         if cid is not None:
             self.cid = cid
         if metadata is not None:
             self.metadata = metadata
         if name is not None:
             self.name = name
+        if repo is not None:
+            self.repo = repo
+        if s3 is not None:
+            self.s3 = s3
         if source_path is not None:
             self.source_path = source_path
         if storage_source is not None:
             self.storage_source = storage_source
         if url is not None:
             self.url = url
         if path is not None:
@@ -138,14 +148,58 @@
         :param name: The name of this StorageSpec.  # noqa: E501
         :type: str
         """
 
         self._name = name
 
     @property
+    def repo(self):
+        """Gets the repo of this StorageSpec.  # noqa: E501
+
+        URL of the git Repo to clone  # noqa: E501
+
+        :return: The repo of this StorageSpec.  # noqa: E501
+        :rtype: str
+        """
+        return self._repo
+
+    @repo.setter
+    def repo(self, repo):
+        """Sets the repo of this StorageSpec.
+
+        URL of the git Repo to clone  # noqa: E501
+
+        :param repo: The repo of this StorageSpec.  # noqa: E501
+        :type: str
+        """
+
+        self._repo = repo
+
+    @property
+    def s3(self):
+        """Gets the s3 of this StorageSpec.  # noqa: E501
+
+
+        :return: The s3 of this StorageSpec.  # noqa: E501
+        :rtype: S3StorageSpec
+        """
+        return self._s3
+
+    @s3.setter
+    def s3(self, s3):
+        """Sets the s3 of this StorageSpec.
+
+
+        :param s3: The s3 of this StorageSpec.  # noqa: E501
+        :type: S3StorageSpec
+        """
+
+        self._s3 = s3
+
+    @property
     def source_path(self):
         """Gets the source_path of this StorageSpec.  # noqa: E501
 
         The path of the host data if we are using local directory paths  # noqa: E501
 
         :return: The source_path of this StorageSpec.  # noqa: E501
         :rtype: str
```

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/submit_request.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/job_create_payload.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,122 +11,120 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class SubmitRequest(object):
+class JobCreatePayload(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'client_public_key': 'str',
-        'job_create_payload': 'list[int]',
-        'signature': 'str'
+        'api_version': 'str',
+        'client_id': 'str',
+        'spec': 'AllOfJobCreatePayloadSpec'
     }
 
     attribute_map = {
-        'client_public_key': 'client_public_key',
-        'job_create_payload': 'job_create_payload',
-        'signature': 'signature'
+        'api_version': 'APIVersion',
+        'client_id': 'ClientID',
+        'spec': 'Spec'
     }
 
-    def __init__(self, client_public_key=None, job_create_payload=None, signature=None):  # noqa: E501
-        """SubmitRequest - a model defined in Swagger"""  # noqa: E501
-        self._client_public_key = None
-        self._job_create_payload = None
-        self._signature = None
+    def __init__(self, api_version=None, client_id=None, spec=None):  # noqa: E501
+        """JobCreatePayload - a model defined in Swagger"""  # noqa: E501
+        self._api_version = None
+        self._client_id = None
+        self._spec = None
         self.discriminator = None
-        self.client_public_key = client_public_key
-        self.job_create_payload = job_create_payload
-        self.signature = signature
+        self.api_version = api_version
+        self.client_id = client_id
+        self.spec = spec
 
     @property
-    def client_public_key(self):
-        """Gets the client_public_key of this SubmitRequest.  # noqa: E501
+    def api_version(self):
+        """Gets the api_version of this JobCreatePayload.  # noqa: E501
 
-        The base64-encoded public key of the client:  # noqa: E501
 
-        :return: The client_public_key of this SubmitRequest.  # noqa: E501
+        :return: The api_version of this JobCreatePayload.  # noqa: E501
         :rtype: str
         """
-        return self._client_public_key
+        return self._api_version
 
-    @client_public_key.setter
-    def client_public_key(self, client_public_key):
-        """Sets the client_public_key of this SubmitRequest.
+    @api_version.setter
+    def api_version(self, api_version):
+        """Sets the api_version of this JobCreatePayload.
 
-        The base64-encoded public key of the client:  # noqa: E501
 
-        :param client_public_key: The client_public_key of this SubmitRequest.  # noqa: E501
+        :param api_version: The api_version of this JobCreatePayload.  # noqa: E501
         :type: str
         """
-        if client_public_key is None:
-            raise ValueError("Invalid value for `client_public_key`, must not be `None`")  # noqa: E501
+        if api_version is None:
+            raise ValueError("Invalid value for `api_version`, must not be `None`")  # noqa: E501
 
-        self._client_public_key = client_public_key
+        self._api_version = api_version
 
     @property
-    def job_create_payload(self):
-        """Gets the job_create_payload of this SubmitRequest.  # noqa: E501
+    def client_id(self):
+        """Gets the client_id of this JobCreatePayload.  # noqa: E501
 
-        The data needed to submit and run a job on the network:  # noqa: E501
+        the id of the client that is submitting the job  # noqa: E501
 
-        :return: The job_create_payload of this SubmitRequest.  # noqa: E501
-        :rtype: list[int]
+        :return: The client_id of this JobCreatePayload.  # noqa: E501
+        :rtype: str
         """
-        return self._job_create_payload
+        return self._client_id
 
-    @job_create_payload.setter
-    def job_create_payload(self, job_create_payload):
-        """Sets the job_create_payload of this SubmitRequest.
+    @client_id.setter
+    def client_id(self, client_id):
+        """Sets the client_id of this JobCreatePayload.
 
-        The data needed to submit and run a job on the network:  # noqa: E501
+        the id of the client that is submitting the job  # noqa: E501
 
-        :param job_create_payload: The job_create_payload of this SubmitRequest.  # noqa: E501
-        :type: list[int]
+        :param client_id: The client_id of this JobCreatePayload.  # noqa: E501
+        :type: str
         """
-        if job_create_payload is None:
-            raise ValueError("Invalid value for `job_create_payload`, must not be `None`")  # noqa: E501
+        if client_id is None:
+            raise ValueError("Invalid value for `client_id`, must not be `None`")  # noqa: E501
 
-        self._job_create_payload = job_create_payload
+        self._client_id = client_id
 
     @property
-    def signature(self):
-        """Gets the signature of this SubmitRequest.  # noqa: E501
+    def spec(self):
+        """Gets the spec of this JobCreatePayload.  # noqa: E501
 
-        A base64-encoded signature of the data, signed by the client:  # noqa: E501
+        The specification of this job.  # noqa: E501
 
-        :return: The signature of this SubmitRequest.  # noqa: E501
-        :rtype: str
+        :return: The spec of this JobCreatePayload.  # noqa: E501
+        :rtype: AllOfJobCreatePayloadSpec
         """
-        return self._signature
+        return self._spec
 
-    @signature.setter
-    def signature(self, signature):
-        """Sets the signature of this SubmitRequest.
+    @spec.setter
+    def spec(self, spec):
+        """Sets the spec of this JobCreatePayload.
 
-        A base64-encoded signature of the data, signed by the client:  # noqa: E501
+        The specification of this job.  # noqa: E501
 
-        :param signature: The signature of this SubmitRequest.  # noqa: E501
-        :type: str
+        :param spec: The spec of this JobCreatePayload.  # noqa: E501
+        :type: AllOfJobCreatePayloadSpec
         """
-        if signature is None:
-            raise ValueError("Invalid value for `signature`, must not be `None`")  # noqa: E501
+        if spec is None:
+            raise ValueError("Invalid value for `spec`, must not be `None`")  # noqa: E501
 
-        self._signature = signature
+        self._spec = spec
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -141,15 +139,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(SubmitRequest, dict):
+        if issubclass(JobCreatePayload, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -157,15 +155,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SubmitRequest):
+        if not isinstance(other, JobCreatePayload):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/submit_response.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/submit_response.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/verification_result.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/verification_result.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/verifier.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/verifier.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/version_request.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/all_ofevents_request_filters.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,62 +10,42 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
+from bacalhau_apiclient.models.event_filter_options import EventFilterOptions  # noqa: F401,E501
 
-class VersionRequest(object):
+class AllOfeventsRequestFilters(EventFilterOptions):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'client_id': 'str'
     }
+    if hasattr(EventFilterOptions, "swagger_types"):
+        swagger_types.update(EventFilterOptions.swagger_types)
 
     attribute_map = {
-        'client_id': 'client_id'
     }
+    if hasattr(EventFilterOptions, "attribute_map"):
+        attribute_map.update(EventFilterOptions.attribute_map)
 
-    def __init__(self, client_id=None):  # noqa: E501
-        """VersionRequest - a model defined in Swagger"""  # noqa: E501
-        self._client_id = None
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """AllOfeventsRequestFilters - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
-        if client_id is not None:
-            self.client_id = client_id
-
-    @property
-    def client_id(self):
-        """Gets the client_id of this VersionRequest.  # noqa: E501
-
-
-        :return: The client_id of this VersionRequest.  # noqa: E501
-        :rtype: str
-        """
-        return self._client_id
-
-    @client_id.setter
-    def client_id(self, client_id):
-        """Sets the client_id of this VersionRequest.
-
-
-        :param client_id: The client_id of this VersionRequest.  # noqa: E501
-        :type: str
-        """
-
-        self._client_id = client_id
+        EventFilterOptions.__init__(self, *args, **kwargs)
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -80,15 +60,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(VersionRequest, dict):
+        if issubclass(AllOfeventsRequestFilters, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +76,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, VersionRequest):
+        if not isinstance(other, AllOfeventsRequestFilters):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `bacalhau_apiclient-0.3.25/bacalhau_apiclient/models/version_response.py` & `bacalhau_apiclient-0.3.26/bacalhau_apiclient/models/version_response.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/docs/BuildVersionInfo.md` & `bacalhau_apiclient-0.3.26/docs/BuildVersionInfo.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/docs/CancelRequest.md` & `bacalhau_apiclient-0.3.26/docs/CancelRequest.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/docs/ComputeNodeInfo.md` & `bacalhau_apiclient-0.3.26/docs/ComputeNodeInfo.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/docs/Deal.md` & `bacalhau_apiclient-0.3.26/docs/Deal.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/docs/ExecutionState.md` & `bacalhau_apiclient-0.3.26/docs/ExecutionState.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # ExecutionState
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
+**accepted_ask_for_bid** | **bool** | Set to true iff the compute node accepted the ask for a bid, and intends to run the job if the bid is accepted by the requester. | [optional] 
 **compute_reference** | **str** | Compute node reference for this job execution | [optional] 
 **create_time** | **str** | CreateTime is the time when the job was created. | [optional] 
 **job_id** | **str** | JobID the job id | [optional] 
 **node_id** | **str** | which node is running this execution | [optional] 
 **published_results** | [**StorageSpec**](StorageSpec.md) |  | [optional] 
 **run_output** | **AllOfExecutionStateRunOutput** | RunOutput of the job | [optional] 
 **state** | **AllOfExecutionStateState** | State is the current state of the execution | [optional]
```

### Comparing `bacalhau_apiclient-0.3.25/docs/HealthApi.md` & `bacalhau_apiclient-0.3.26/docs/HealthApi.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/docs/JobApi.md` & `bacalhau_apiclient-0.3.26/docs/JobApi.md`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 All URIs are relative to *http://bootstrap.production.bacalhau.org:1234/*
 
 Method | HTTP request | Description
 ------------- | ------------- | -------------
 [**cancel**](JobApi.md#cancel) | **POST** /requester/cancel | Cancels the job with the job-id specified in the body payload.
 [**events**](JobApi.md#events) | **POST** /requester/events | Returns the events related to the job-id passed in the body payload. Useful for troubleshooting.
 [**list**](JobApi.md#list) | **POST** /requester/list | Simply lists jobs.
+[**logs**](JobApi.md#logs) | **POST** /requester/logs | Displays the logs for a current job/execution
 [**results**](JobApi.md#results) | **POST** /requester/results | Returns the results of the job-id specified in the body payload.
 [**states**](JobApi.md#states) | **POST** /requester/states | Returns the state of the job-id specified in the body payload.
 [**submit**](JobApi.md#submit) | **POST** /requester/submit | Submits a new job to the network.
 
 # **cancel**
 > CancelResponse cancel(body)
 
@@ -151,14 +152,62 @@
 ### HTTP request headers
 
  - **Content-Type**: application/json
  - **Accept**: application/json
 
 [[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
 
+# **logs**
+> str logs(body)
+
+Displays the logs for a current job/execution
+
+Shows the output from the job specified by `id` as long as that job belongs to `client_id`.  The ouput will be continuous until either, the client disconnects or the execution completes.
+
+### Example
+```python
+from __future__ import print_function
+import time
+import bacalhau_apiclient
+from bacalhau_apiclient.rest import ApiException
+from pprint import pprint
+
+# create an instance of the API class
+api_instance = bacalhau_apiclient.JobApi()
+body = bacalhau_apiclient.LogRequest() # LogRequest | 
+
+try:
+    # Displays the logs for a current job/execution
+    api_response = api_instance.logs(body)
+    pprint(api_response)
+except ApiException as e:
+    print("Exception when calling JobApi->logs: %s\n" % e)
+```
+
+### Parameters
+
+Name | Type | Description  | Notes
+------------- | ------------- | ------------- | -------------
+ **body** | [**LogRequest**](LogRequest.md)|  | 
+
+### Return type
+
+**str**
+
+### Authorization
+
+No authorization required
+
+### HTTP request headers
+
+ - **Content-Type**: application/json
+ - **Accept**: application/json
+
+[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
+
 # **results**
 > ResultsResponse results(body)
 
 Returns the results of the job-id specified in the body payload.
 
 Example response:  ```json {   \"results\": [     {       \"NodeID\": \"QmdZQ7ZbhnvWY1J12XYKGHApJ6aufKyLNSvf8jZBrBaAVL\",       \"Data\": {         \"StorageSource\": \"IPFS\",         \"Name\": \"job-9304c616-291f-41ad-b862-54e133c0149e-shard-0-host-QmdZQ7ZbhnvWY1J12XYKGHApJ6aufKyLNSvf8jZBrBaAVL\",         \"CID\": \"QmTVmC7JBD2ES2qGPqBNVWnX1KeEPNrPGb7rJ8cpFgtefe\"       }     }   ] } ```
 
@@ -252,15 +301,15 @@
 [[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
 
 # **submit**
 > SubmitResponse submit(body)
 
 Submits a new job to the network.
 
-Description:  * `client_public_key`: The base64-encoded public key of the client. * `signature`: A base64-encoded signature of the `data` attribute, signed by the client. * `job_create_payload`:     * `ClientID`: Request must specify a `ClientID`. To retrieve your `ClientID`, you can do the following: (1) submit a dummy job to Bacalhau (or use one you created before), (2) run `bacalhau describe <job-id>` and fetch the `ClientID` field.  * `APIVersion`: e.g. `\"V1beta1\"`.     * `Spec`: https://github.com/bacalhau-project/bacalhau/blob/main/pkg/job.go 
+Description:  * `client_public_key`: The base64-encoded public key of the client. * `signature`: A base64-encoded signature of the `data` attribute, signed by the client. * `payload`:     * `ClientID`: Request must specify a `ClientID`. To retrieve your `ClientID`, you can do the following: (1) submit a dummy job to Bacalhau (or use one you created before), (2) run `bacalhau describe <job-id>` and fetch the `ClientID` field.  * `APIVersion`: e.g. `\"V1beta1\"`.     * `Spec`: https://github.com/bacalhau-project/bacalhau/blob/main/pkg/job.go 
 
 ### Example
 ```python
 from __future__ import print_function
 import time
 import bacalhau_apiclient
 from bacalhau_apiclient.rest import ApiException
```

### Comparing `bacalhau_apiclient-0.3.25/docs/JobCancelPayload.md` & `bacalhau_apiclient-0.3.26/docs/JobCancelPayload.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/docs/JobHistory.md` & `bacalhau_apiclient-0.3.26/docs/JobHistory.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/docs/JobRequester.md` & `bacalhau_apiclient-0.3.26/docs/JobRequester.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/docs/JobSpecDocker.md` & `bacalhau_apiclient-0.3.26/docs/JobSpecDocker.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/docs/JobSpecLanguage.md` & `bacalhau_apiclient-0.3.26/docs/JobSpecLanguage.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/docs/JobSpecWasm.md` & `bacalhau_apiclient-0.3.26/docs/JobSpecWasm.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/docs/JobState.md` & `bacalhau_apiclient-0.3.26/docs/JobState.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/docs/JobWithInfo.md` & `bacalhau_apiclient-0.3.26/docs/JobWithInfo.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/docs/LabelSelectorRequirement.md` & `bacalhau_apiclient-0.3.26/docs/LabelSelectorRequirement.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/docs/ListRequest.md` & `bacalhau_apiclient-0.3.26/docs/ListRequest.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/docs/Metadata.md` & `bacalhau_apiclient-0.3.26/docs/Metadata.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/docs/MiscApi.md` & `bacalhau_apiclient-0.3.26/docs/MiscApi.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/docs/NodeInfo.md` & `bacalhau_apiclient-0.3.26/docs/NodeInfo.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/docs/ResourceUsageConfig.md` & `bacalhau_apiclient-0.3.26/docs/ResourceUsageConfig.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/docs/RunCommandResult.md` & `bacalhau_apiclient-0.3.26/docs/RunCommandResult.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/docs/Spec.md` & `bacalhau_apiclient-0.3.26/docs/Spec.md`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 **deal** | **AllOfSpecDeal** | The deal the client has made, such as which job bids they have accepted. | [optional] 
 **do_not_track** | **bool** | Do not track specified by the client | [optional] 
 **docker** | **AllOfSpecDocker** | executor specific data | [optional] 
 **engine** | **AllOfSpecEngine** | e.g. docker or language | [optional] 
 **language** | [**JobSpecLanguage**](JobSpecLanguage.md) |  | [optional] 
 **network** | **AllOfSpecNetwork** | The type of networking access that the job needs | [optional] 
 **node_selectors** | [**list[LabelSelectorRequirement]**](LabelSelectorRequirement.md) | NodeSelectors is a selector which must be true for the compute node to run this job. | [optional] 
-**publisher** | **AllOfSpecPublisher** | there can be multiple publishers for the job | [optional] 
+**publisher** | **AllOfSpecPublisher** | there can be multiple publishers for the job deprecated: use PublisherSpec instead | [optional] 
+**publisher_spec** | [**PublisherSpec**](PublisherSpec.md) |  | [optional] 
 **resources** | **AllOfSpecResources** | the compute (cpu, ram) resources this job requires | [optional] 
 **timeout** | **float** | How long a job can run in seconds before it is killed. This includes the time required to run, verify and publish results | [optional] 
 **verifier** | [**Verifier**](Verifier.md) |  | [optional] 
 **wasm** | [**JobSpecWasm**](JobSpecWasm.md) |  | [optional] 
 **inputs** | [**list[StorageSpec]**](StorageSpec.md) | the data volumes we will read in the job for example \&quot;read this ipfs cid\&quot; TODO: #667 Replace with \&quot;Inputs\&quot;, \&quot;Outputs\&quot; (note the caps) for yaml/json when we update the n.js file | [optional] 
 **outputs** | [**list[StorageSpec]**](StorageSpec.md) | the data volumes we will write in the job for example \&quot;write the results to ipfs\&quot; | [optional]
```

### Comparing `bacalhau_apiclient-0.3.25/docs/StorageSpec.md` & `bacalhau_apiclient-0.3.26/docs/StorageSpec.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
 **cid** | **str** | The unique ID of the data, where it makes sense (for example, in an IPFS storage spec this will be the data&#x27;s CID). NOTE: The below is capitalized to match IPFS &amp; IPLD (even though it&#x27;s out of golang fmt) | [optional] 
 **metadata** | **dict(str, str)** | Additional properties specific to each driver | [optional] 
 **name** | **str** | Name of the spec&#x27;s data, for reference. | [optional] 
+**repo** | **str** | URL of the git Repo to clone | [optional] 
+**s3** | [**S3StorageSpec**](S3StorageSpec.md) |  | [optional] 
 **source_path** | **str** | The path of the host data if we are using local directory paths | [optional] 
 **storage_source** | **AllOfStorageSpecStorageSource** | StorageSource is the abstract source of the data. E.g. a storage source might be a URL download, but doesn&#x27;t specify how the execution engine does the download or what it will do with the downloaded data. | [optional] 
 **url** | **str** | Source URL of the data | [optional] 
 **path** | **str** | The path that the spec&#x27;s data should be mounted on, where it makes sense (for example, in a Docker storage spec this will be a filesystem path). TODO: #668 Replace with \&quot;Path\&quot; (note the caps) for yaml/json when we update the n.js file | [optional] 
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `bacalhau_apiclient-0.3.25/docs/SubmitRequest.md` & `bacalhau_apiclient-0.3.26/docs/LogRequest.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# SubmitRequest
+# LogRequest
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
 **client_public_key** | **str** | The base64-encoded public key of the client: | 
-**job_create_payload** | **list[int]** | The data needed to submit and run a job on the network: | 
+**payload** | **AllOflogRequestPayload** | The data needed to cancel a running job on the network | 
 **signature** | **str** | A base64-encoded signature of the data, signed by the client: | 
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `bacalhau_apiclient-0.3.25/docs/UtilsApi.md` & `bacalhau_apiclient-0.3.26/docs/UtilsApi.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/.gitignore` & `bacalhau_apiclient-0.3.26/.gitignore`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/LICENSE` & `bacalhau_apiclient-0.3.26/LICENSE`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-0.3.25/README.md` & `bacalhau_apiclient-0.3.26/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # bacalhau_apiclient
 This page is the reference of the Bacalhau REST API. Project docs are available at https://docs.bacalhau.org/. Find more information about Bacalhau at https://github.com/bacalhau-project/bacalhau.
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
 - API version: ${PYPI_VERSION}
-- Package version: 0.3.25
+- Package version: 0.3.26
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 For more information, please visit [https://github.com/bacalhau-project/bacalhau](https://github.com/bacalhau-project/bacalhau)
 
 ## Requirements.
 
 Python 3.6+
 
@@ -80,31 +80,34 @@
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *HealthApi* | [**api_serverdebug**](docs/HealthApi.md#api_serverdebug) | **GET** /debug | Returns debug information on what the current node is doing.
 *HealthApi* | [**debug**](docs/HealthApi.md#debug) | **GET** /requester/debug | Returns debug information on what the current node is doing.
 *JobApi* | [**cancel**](docs/JobApi.md#cancel) | **POST** /requester/cancel | Cancels the job with the job-id specified in the body payload.
 *JobApi* | [**events**](docs/JobApi.md#events) | **POST** /requester/events | Returns the events related to the job-id passed in the body payload. Useful for troubleshooting.
 *JobApi* | [**list**](docs/JobApi.md#list) | **POST** /requester/list | Simply lists jobs.
+*JobApi* | [**logs**](docs/JobApi.md#logs) | **POST** /requester/logs | Displays the logs for a current job/execution
 *JobApi* | [**results**](docs/JobApi.md#results) | **POST** /requester/results | Returns the results of the job-id specified in the body payload.
 *JobApi* | [**states**](docs/JobApi.md#states) | **POST** /requester/states | Returns the state of the job-id specified in the body payload.
 *JobApi* | [**submit**](docs/JobApi.md#submit) | **POST** /requester/submit | Submits a new job to the network.
 *MiscApi* | [**api_serverversion**](docs/MiscApi.md#api_serverversion) | **POST** /version | Returns the build version running on the server.
 *UtilsApi* | [**healthz**](docs/UtilsApi.md#healthz) | **GET** /healthz | 
 *UtilsApi* | [**id**](docs/UtilsApi.md#id) | **GET** /id | Returns the id of the host node.
 *UtilsApi* | [**livez**](docs/UtilsApi.md#livez) | **GET** /livez | 
 *UtilsApi* | [**logz**](docs/UtilsApi.md#logz) | **GET** /logz | 
 *UtilsApi* | [**node_info**](docs/UtilsApi.md#node_info) | **GET** /node_info | Returns the info of the node.
 *UtilsApi* | [**peers**](docs/UtilsApi.md#peers) | **GET** /peers | Returns the peers connected to the host via the transport layer.
 *UtilsApi* | [**readyz**](docs/UtilsApi.md#readyz) | **GET** /readyz | 
 *UtilsApi* | [**varz**](docs/UtilsApi.md#varz) | **GET** /varz | 
+*DefaultApi* | [**api_serverapprover**](docs/DefaultApi.md#api_serverapprover) | **GET** /approve | Approves a job to be run on this compute node.
 
 ## Documentation For Models
 
  - [AllOfExecutionStateRunOutput](docs/AllOfExecutionStateRunOutput.md)
  - [AllOfExecutionStateState](docs/AllOfExecutionStateState.md)
+ - [AllOfJobCreatePayloadSpec](docs/AllOfJobCreatePayloadSpec.md)
  - [AllOfJobSpec](docs/AllOfJobSpec.md)
  - [AllOfJobSpecLanguageJobContext](docs/AllOfJobSpecLanguageJobContext.md)
  - [AllOfJobSpecWasmEntryModule](docs/AllOfJobSpecWasmEntryModule.md)
  - [AllOfJobStateState](docs/AllOfJobStateState.md)
  - [AllOfJobWithInfoJob](docs/AllOfJobWithInfoJob.md)
  - [AllOfJobWithInfoState](docs/AllOfJobWithInfoState.md)
  - [AllOfLabelSelectorRequirementOperator](docs/AllOfLabelSelectorRequirementOperator.md)
@@ -112,53 +115,62 @@
  - [AllOfSpecDocker](docs/AllOfSpecDocker.md)
  - [AllOfSpecEngine](docs/AllOfSpecEngine.md)
  - [AllOfSpecNetwork](docs/AllOfSpecNetwork.md)
  - [AllOfSpecPublisher](docs/AllOfSpecPublisher.md)
  - [AllOfSpecResources](docs/AllOfSpecResources.md)
  - [AllOfStorageSpecStorageSource](docs/AllOfStorageSpecStorageSource.md)
  - [AllOfcancelRequestPayload](docs/AllOfcancelRequestPayload.md)
+ - [AllOfeventsRequestFilters](docs/AllOfeventsRequestFilters.md)
+ - [AllOflogRequestPayload](docs/AllOflogRequestPayload.md)
+ - [AllOfsubmitRequestPayload](docs/AllOfsubmitRequestPayload.md)
  - [BuildVersionInfo](docs/BuildVersionInfo.md)
  - [CancelRequest](docs/CancelRequest.md)
  - [CancelResponse](docs/CancelResponse.md)
  - [ComputeNodeInfo](docs/ComputeNodeInfo.md)
  - [Deal](docs/Deal.md)
  - [Engine](docs/Engine.md)
+ - [EventFilterOptions](docs/EventFilterOptions.md)
  - [EventsRequest](docs/EventsRequest.md)
  - [EventsResponse](docs/EventsResponse.md)
  - [ExecutionState](docs/ExecutionState.md)
  - [ExecutionStateType](docs/ExecutionStateType.md)
  - [FreeSpace](docs/FreeSpace.md)
  - [HealthInfo](docs/HealthInfo.md)
  - [Job](docs/Job.md)
  - [JobCancelPayload](docs/JobCancelPayload.md)
+ - [JobCreatePayload](docs/JobCreatePayload.md)
  - [JobHistory](docs/JobHistory.md)
  - [JobHistoryType](docs/JobHistoryType.md)
  - [JobRequester](docs/JobRequester.md)
  - [JobSpecDocker](docs/JobSpecDocker.md)
  - [JobSpecLanguage](docs/JobSpecLanguage.md)
  - [JobSpecWasm](docs/JobSpecWasm.md)
  - [JobState](docs/JobState.md)
  - [JobStateType](docs/JobStateType.md)
  - [JobWithInfo](docs/JobWithInfo.md)
  - [LabelSelectorRequirement](docs/LabelSelectorRequirement.md)
  - [ListRequest](docs/ListRequest.md)
  - [ListResponse](docs/ListResponse.md)
+ - [LogRequest](docs/LogRequest.md)
+ - [LogsPayload](docs/LogsPayload.md)
  - [Metadata](docs/Metadata.md)
  - [MountStatus](docs/MountStatus.md)
  - [Network](docs/Network.md)
  - [NetworkConfig](docs/NetworkConfig.md)
  - [NodeInfo](docs/NodeInfo.md)
  - [NodeType](docs/NodeType.md)
  - [PeerAddrInfo](docs/PeerAddrInfo.md)
  - [PublishedResult](docs/PublishedResult.md)
  - [Publisher](docs/Publisher.md)
+ - [PublisherSpec](docs/PublisherSpec.md)
  - [ResourceUsageConfig](docs/ResourceUsageConfig.md)
  - [ResourceUsageData](docs/ResourceUsageData.md)
  - [ResultsResponse](docs/ResultsResponse.md)
  - [RunCommandResult](docs/RunCommandResult.md)
+ - [S3StorageSpec](docs/S3StorageSpec.md)
  - [SelectionOperator](docs/SelectionOperator.md)
  - [Spec](docs/Spec.md)
  - [StateChangeExecutionStateType](docs/StateChangeExecutionStateType.md)
  - [StateChangeJobStateType](docs/StateChangeJobStateType.md)
  - [StateRequest](docs/StateRequest.md)
  - [StateResponse](docs/StateResponse.md)
  - [StorageSourceType](docs/StorageSourceType.md)
```

### Comparing `bacalhau_apiclient-0.3.25/pyproject.toml` & `bacalhau_apiclient-0.3.26/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bacalhau_apiclient"
-version = "0.3.25"
+version = "0.3.26"
 authors = [
 { name="Enrico Rotundo", email="enrico.rotundo@gmail.com" },
 ]
 description = "A Python client for the Bacalhau public API - https://github.com/bacalhau-project/bacalhau/tree/main/clients/python"
 readme = "README.md"
 requires-python = ">=3.6.2"
 classifiers = [
```

### Comparing `bacalhau_apiclient-0.3.25/PKG-INFO` & `bacalhau_apiclient-0.3.26/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacalhau_apiclient
-Version: 0.3.25
+Version: 0.3.26
 Summary: A Python client for the Bacalhau public API - https://github.com/bacalhau-project/bacalhau/tree/main/clients/python
 Project-URL: Homepage, https://github.com/bacalhau-project/bacalhau/
 Project-URL: Bug Tracker, https://github.com/bacalhau-project/bacalhau/issues
 Author-email: Enrico Rotundo <enrico.rotundo@gmail.com>
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 
 # bacalhau_apiclient
 This page is the reference of the Bacalhau REST API. Project docs are available at https://docs.bacalhau.org/. Find more information about Bacalhau at https://github.com/bacalhau-project/bacalhau.
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
 - API version: ${PYPI_VERSION}
-- Package version: 0.3.25
+- Package version: 0.3.26
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 For more information, please visit [https://github.com/bacalhau-project/bacalhau](https://github.com/bacalhau-project/bacalhau)
 
 ## Requirements.
 
 Python 3.6+
 
@@ -93,31 +93,34 @@
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *HealthApi* | [**api_serverdebug**](docs/HealthApi.md#api_serverdebug) | **GET** /debug | Returns debug information on what the current node is doing.
 *HealthApi* | [**debug**](docs/HealthApi.md#debug) | **GET** /requester/debug | Returns debug information on what the current node is doing.
 *JobApi* | [**cancel**](docs/JobApi.md#cancel) | **POST** /requester/cancel | Cancels the job with the job-id specified in the body payload.
 *JobApi* | [**events**](docs/JobApi.md#events) | **POST** /requester/events | Returns the events related to the job-id passed in the body payload. Useful for troubleshooting.
 *JobApi* | [**list**](docs/JobApi.md#list) | **POST** /requester/list | Simply lists jobs.
+*JobApi* | [**logs**](docs/JobApi.md#logs) | **POST** /requester/logs | Displays the logs for a current job/execution
 *JobApi* | [**results**](docs/JobApi.md#results) | **POST** /requester/results | Returns the results of the job-id specified in the body payload.
 *JobApi* | [**states**](docs/JobApi.md#states) | **POST** /requester/states | Returns the state of the job-id specified in the body payload.
 *JobApi* | [**submit**](docs/JobApi.md#submit) | **POST** /requester/submit | Submits a new job to the network.
 *MiscApi* | [**api_serverversion**](docs/MiscApi.md#api_serverversion) | **POST** /version | Returns the build version running on the server.
 *UtilsApi* | [**healthz**](docs/UtilsApi.md#healthz) | **GET** /healthz | 
 *UtilsApi* | [**id**](docs/UtilsApi.md#id) | **GET** /id | Returns the id of the host node.
 *UtilsApi* | [**livez**](docs/UtilsApi.md#livez) | **GET** /livez | 
 *UtilsApi* | [**logz**](docs/UtilsApi.md#logz) | **GET** /logz | 
 *UtilsApi* | [**node_info**](docs/UtilsApi.md#node_info) | **GET** /node_info | Returns the info of the node.
 *UtilsApi* | [**peers**](docs/UtilsApi.md#peers) | **GET** /peers | Returns the peers connected to the host via the transport layer.
 *UtilsApi* | [**readyz**](docs/UtilsApi.md#readyz) | **GET** /readyz | 
 *UtilsApi* | [**varz**](docs/UtilsApi.md#varz) | **GET** /varz | 
+*DefaultApi* | [**api_serverapprover**](docs/DefaultApi.md#api_serverapprover) | **GET** /approve | Approves a job to be run on this compute node.
 
 ## Documentation For Models
 
  - [AllOfExecutionStateRunOutput](docs/AllOfExecutionStateRunOutput.md)
  - [AllOfExecutionStateState](docs/AllOfExecutionStateState.md)
+ - [AllOfJobCreatePayloadSpec](docs/AllOfJobCreatePayloadSpec.md)
  - [AllOfJobSpec](docs/AllOfJobSpec.md)
  - [AllOfJobSpecLanguageJobContext](docs/AllOfJobSpecLanguageJobContext.md)
  - [AllOfJobSpecWasmEntryModule](docs/AllOfJobSpecWasmEntryModule.md)
  - [AllOfJobStateState](docs/AllOfJobStateState.md)
  - [AllOfJobWithInfoJob](docs/AllOfJobWithInfoJob.md)
  - [AllOfJobWithInfoState](docs/AllOfJobWithInfoState.md)
  - [AllOfLabelSelectorRequirementOperator](docs/AllOfLabelSelectorRequirementOperator.md)
@@ -125,53 +128,62 @@
  - [AllOfSpecDocker](docs/AllOfSpecDocker.md)
  - [AllOfSpecEngine](docs/AllOfSpecEngine.md)
  - [AllOfSpecNetwork](docs/AllOfSpecNetwork.md)
  - [AllOfSpecPublisher](docs/AllOfSpecPublisher.md)
  - [AllOfSpecResources](docs/AllOfSpecResources.md)
  - [AllOfStorageSpecStorageSource](docs/AllOfStorageSpecStorageSource.md)
  - [AllOfcancelRequestPayload](docs/AllOfcancelRequestPayload.md)
+ - [AllOfeventsRequestFilters](docs/AllOfeventsRequestFilters.md)
+ - [AllOflogRequestPayload](docs/AllOflogRequestPayload.md)
+ - [AllOfsubmitRequestPayload](docs/AllOfsubmitRequestPayload.md)
  - [BuildVersionInfo](docs/BuildVersionInfo.md)
  - [CancelRequest](docs/CancelRequest.md)
  - [CancelResponse](docs/CancelResponse.md)
  - [ComputeNodeInfo](docs/ComputeNodeInfo.md)
  - [Deal](docs/Deal.md)
  - [Engine](docs/Engine.md)
+ - [EventFilterOptions](docs/EventFilterOptions.md)
  - [EventsRequest](docs/EventsRequest.md)
  - [EventsResponse](docs/EventsResponse.md)
  - [ExecutionState](docs/ExecutionState.md)
  - [ExecutionStateType](docs/ExecutionStateType.md)
  - [FreeSpace](docs/FreeSpace.md)
  - [HealthInfo](docs/HealthInfo.md)
  - [Job](docs/Job.md)
  - [JobCancelPayload](docs/JobCancelPayload.md)
+ - [JobCreatePayload](docs/JobCreatePayload.md)
  - [JobHistory](docs/JobHistory.md)
  - [JobHistoryType](docs/JobHistoryType.md)
  - [JobRequester](docs/JobRequester.md)
  - [JobSpecDocker](docs/JobSpecDocker.md)
  - [JobSpecLanguage](docs/JobSpecLanguage.md)
  - [JobSpecWasm](docs/JobSpecWasm.md)
  - [JobState](docs/JobState.md)
  - [JobStateType](docs/JobStateType.md)
  - [JobWithInfo](docs/JobWithInfo.md)
  - [LabelSelectorRequirement](docs/LabelSelectorRequirement.md)
  - [ListRequest](docs/ListRequest.md)
  - [ListResponse](docs/ListResponse.md)
+ - [LogRequest](docs/LogRequest.md)
+ - [LogsPayload](docs/LogsPayload.md)
  - [Metadata](docs/Metadata.md)
  - [MountStatus](docs/MountStatus.md)
  - [Network](docs/Network.md)
  - [NetworkConfig](docs/NetworkConfig.md)
  - [NodeInfo](docs/NodeInfo.md)
  - [NodeType](docs/NodeType.md)
  - [PeerAddrInfo](docs/PeerAddrInfo.md)
  - [PublishedResult](docs/PublishedResult.md)
  - [Publisher](docs/Publisher.md)
+ - [PublisherSpec](docs/PublisherSpec.md)
  - [ResourceUsageConfig](docs/ResourceUsageConfig.md)
  - [ResourceUsageData](docs/ResourceUsageData.md)
  - [ResultsResponse](docs/ResultsResponse.md)
  - [RunCommandResult](docs/RunCommandResult.md)
+ - [S3StorageSpec](docs/S3StorageSpec.md)
  - [SelectionOperator](docs/SelectionOperator.md)
  - [Spec](docs/Spec.md)
  - [StateChangeExecutionStateType](docs/StateChangeExecutionStateType.md)
  - [StateChangeJobStateType](docs/StateChangeJobStateType.md)
  - [StateRequest](docs/StateRequest.md)
  - [StateResponse](docs/StateResponse.md)
  - [StorageSourceType](docs/StorageSourceType.md)
```

