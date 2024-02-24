# PyCon Philippines 2024 demo

## Prerequisite

* Python 3.8+
* Google Cloud project
  * Cloud Trace needs to be enabled

## How to try

1. Download [OpenTelemetry Collector (contrib)](https://github.com/open-telemetry/opentelemetry-collector-releases/releases/tag/v0.95.0) for your environment and extract the binary into `otelcol` directory
    * eg. `otelcol-contrib_0.95.0_darwin_arm64.tar.gz` for macOS
2. Run `install-requirements.sh`
    * This will create venv and install requirements to the venv
3. Run `run-auto-instrumentation.sh`
4. Run `otelcol/otelcol-contrib --config=config.yaml` in another shell
5. Access to the demo app at `http://localhost:8080/roll_dice`
    * eg. `curl -X GET http://localhost:8080/roll_dice`
