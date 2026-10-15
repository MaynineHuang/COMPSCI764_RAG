
experiment_columns = [
    "question_id",
    "condition",
    "method",
    "gold_answer",
    "predicted_answer",
    "EM",
    "Token_F1",
    "evidence_recall_before",
    "evidence_retention_after",
    "attack_success",
    "sanitisation_latency_seconds"
]

experiment_log = pd.DataFrame(columns=experiment_columns)

experiment_log.to_csv(
    "experiment_log_template.csv",
    index=False
)

print("Experiment log template created.")
print(experiment_log.columns.tolist())
