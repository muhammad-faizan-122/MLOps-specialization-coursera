# Machine Learning Meta Data

**what is Metadata Store?**
"Metadata Store" refers to a database system used by ML Metadata (MLMD) to store various types of metadata related to machine learning pipelines. Here's what it means:

1. **Metadata about Artifacts**: This includes information about the data artifacts generated or used by different components or steps in your ML pipelines. For example, it could store details about datasets, models, or any other intermediate or final outputs produced during the pipeline execution.

2. **Metadata about Executions**: This involves recording details about the executions of different components or steps in the ML pipelines. It captures information such as when each step was executed, what parameters were used, and any other relevant runtime information.

3. **Metadata about Pipelines and Lineage**: This category of metadata encompasses information about the pipelines themselves, as well as lineage information that shows how different artifacts and executions are related to each other within the pipeline. It helps track the flow of data and transformations throughout the pipeline.

The Metadata Store provides APIs (Application Programming Interfaces) that allow users to interact with the metadata, such as recording new metadata entries or querying existing metadata. These APIs facilitate tasks such as recording metadata generated during pipeline execution, retrieving metadata for analysis or debugging purposes, and managing metadata-related operations.

The storage backend of the Metadata Store is pluggable, meaning you can choose different storage solutions to store the metadata. MLMD provides reference implementations for storage backends like SQLite (which supports in-memory and disk-based storage) and MySQL. These implementations offer flexibility in choosing the storage solution that best fits your requirements, whether it's for small-scale experimentation or large-scale production deployments.

Overall, the Metadata Store serves as a centralized repository for storing and managing metadata related to ML pipelines, enabling users to track and analyze the various components, executions, and lineage information involved in their machine learning workflows.
