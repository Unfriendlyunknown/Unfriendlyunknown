- 👋 Hi, I’m @Unfriendlyunknown
- 👀 I’m interested in ...
- 😋 I’m currently learning ...
- ✅️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
423 358 5303
<!---
Unfriendlyunknown/Unfriendlyunknown is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
Mary Ann webb doxbin 
            } else {
                final ProcessState proc = act.getAssociationState().getProcess();
                if (proc != null) {
                    final int procState = proc.getCombinedState() % STATE_COUNT;
                    if (act.mProcState == procState) {
                        act.startActive(now);
                    } else {
                        act.stopActive(now);
                        if (act.mProcState < procState) {
                            Slog.w(TAG, "Tracking association " + act + " whose proc state "
                                    + act.mProcState + " is better than process " + proc
                                    + " proc state " + procState);
                        }
                    }
                    
                } else {
