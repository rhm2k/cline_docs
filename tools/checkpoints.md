# Checkpoints

Checkpoints automatically save snapshots of your workspace after each step in a task. This powerful feature lets you:

- Track and review changes made during a task
- Roll back to any previous point if needed
- Experiment confidently with auto-approve mode
- Maintain full control over your workspace

## How Checkpoints Work

Cline creates a checkpoint after each tool use (file edits, commands, etc.). These checkpoints:

- Work alongside your Git workflow without interference
- Have minimal performance impact
- Handle large codebases efficiently
- Maintain context between restores
- Use a shadow Git repository to track changes


### Viewing Changes & Restoring to Checkpoint

After each **Edit** or **Create** tool use, you can:

1. Click the "Compare" button to see modified files
2. Click the "Restore" button to open restore options

![Checkpoint Buttons](assets/CheckpointsButtons.png)

### Rolling Back

To restore to a previous point:

1. Click the "Restore" button next to any step
2. Choose from three options:
   - **Restore Task and Workspace**: Reset both codebase and task to that point
   - **Restore Task Only**: Keep codebase changes but revert task context
   - **Restore Workspace Only**: Reset codebase while preserving task context

## Use Cases

Checkpoints let you be more experimental with Cline. While human coding is often methodical and iterative, AI can make substantial changes quickly. Checkpoints help you track these changes and revert if needed.

### 1. Using Auto-Approve Mode
- Provides safety net for rapid iterations
- Makes it easy to undo unexpected results

### 2. Testing Different Approaches
- Try multiple solutions confidently
- Compare different implementations
- Quickly revert to working states

![Checkpoints Demo](assets/checkpointsDemo.gif)


## Best Practices

1. Review changes regularly
2. Use checkpoints as safety nets
3. Leverage auto-approve mode confidently
4. Restore selectively based on needs
5. Clean up old checkpoints periodically

Checkpoints make Cline more powerful and reliable, giving you peace of mind and control over your workspace.
