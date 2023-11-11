# NHK2024_mbd_TestMotorControl
旧基板とモタドラ (A相) を利用してエンコーダからのフィードバックから回すやつ(制御周期1000Hz)

20Hzでuartで回転速度(Pulse/1ms), Duty比を返す

グローバル変数"setpoint"を書き換えて目標値を変更

グローバル変数"KP,KI,KD"がPIDのパラメータ

マクロ"MOTOR_POLARITY"を0か1に設定することで，モーターの回転方向の設定

マクロ"ENC_POLARITY"を0か1に設定して，エンコーダの数値の正負を反転

マクロ"DEBUG"をコメントアウトするとuartによる出力がなくなる
