# Packcress 1.0 TEST
Native Android 0/1knapsack selection puzzle. Android8+ min26/target35. Package com.gg007.packcress.

## Rules
Choose from eight distinct items A-H. Each row shows weight and reward. Tap any item row to take it or leave it; each item can be taken at most once, with no fractions. Keep the total weight at or below the printed capacity and maximize total reward. Capacity need not be filled exactly. Overweight selections are allowed while editing but CHECK PACK rejects them. Press CHECK explicitly. Twelve original boards, one highest-reward subset each; reward-per-weight greedy fails on every board. Weights and rewards are abstract puzzle units, not kilograms or money. Undo/reset and saved palette/optional item letters.

## Download and status
https://mega.co.nz/#!cUcSGLRY!BTkBkaPgUY6hBqwpZR1DzB4-W8t-3Lq_B4oD6ILQD-0
APK16878bytes; SHA256282d9b4b900e8ca4589644a81b0e64d139258dd919298fdb9191257329d61719. Original certificate SHA2561651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. No requested permissions. GG007 icon unchanged. Anonymous downloaded bytes exact.

## Checks
Independent exhaustive subset enumeration checks all 256 subsets per board,3072 total, against production descending-capacity 0/1 dynamic programming. Another 732 capacity checks,2000 random instances and 24576 toggle/undo/clear cases pass. Every original board has a unique best subset and a worse reward-per-weight greedy result. Empty/single/overweight/no-reuse/tied optimum/bounds cases pass. Twelve actual row-choice/CHECK optimum tap-solves, empty/overweight/greedy rejection, clear/undo/reset, solved locks, NEXT, levels/menu/privacy and saved palette/item letters pass. Twenty drawing previews visually inspected, not phone screenshots. Original signing certificate/icon unchanged, no permissions. Anonymous APK bytes match. Phone runtime/performance/external-browser QA and full Git source commit remain incomplete. Signed TEST, not final or Play published.

## Functional difference
Current 241 studio descriptions and 803 legacy descriptions reviewed. Slotcress maximizes reward among non-overlapping fixed intervals. Covercress selects finite bundles covering a union; Mintcress reuses unlimited denominations to make an exact target with fewest pieces. Packcress instead takes or leaves each distinct item once, limits summed weight by capacity and maximizes reward, allowing unused capacity. Legacy CutQueue fits required cuts into stock; it does not choose reward-bearing items. No matching factory mechanic found. Known 0/1 knapsack adaptation, not a globally new algorithm. Original seeded item tables, native implementation and row-choice interaction.

## Build and tests
JDK17/AndroidSDK35/build-tools35.0.0. python generate-levels.py reproduces levels.json. javac -d /tmp/mint-test src/com/gg007/packcress/Board.java BoardTest.java then java -cp /tmp/mint-test com.gg007.packcress.BoardTest. bash build.sh produces an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to private signing material. No signing secret included. adapter/android is the Java2D drawing adapter used with PackAdapterTest.java, not an Android runtime.

## Privacy and branding
Packcress runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Palette, item-letter labels and solved-level marks stay in this app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 menu, original icon, studio https://ilanis-agent.github.io/gg-007-gaming/ and privacy.

## Preservation and publishing
Complete source/APK/exact cumulative242cardstudio/publishing fragments privately preserved:
https://files.instinct.com/slsbqkl91ns9-packcress-source-archive
https://github.com/iLanis-agent/packcress holds README only; full Git source pending. All four studio includes and Pages settings unchanged. Both sites verified separately.

## Rule sources
https://faculty.cc.gatech.edu/~ladha/algo/L12.pdf
https://student.cs.uwaterloo.ca/~cs341/lectures/lecture07.pdf
https://www.cs.cmu.edu/~ckingsf/class/02713/lectures/lec16-subsetsum.pdf
https://www.cs.ox.ac.uk/files/12572/dynamic.pdf
https://www.cs.miami.edu/home/odelia/teaching/csc317.sp15/syllabus/Algorithms8bClass_greedy.pdf
https://en.wikipedia.org/wiki/Knapsack_problem
