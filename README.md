# Arrie-Muhammad-Aries-Sharief---Tugas-2
Daftar Bug

High : Debugging GameManager.cs, variable _score++ bermasalah di ganti dengan score++; dan score di jadikan string; solusi _(underscore) symbol di hapus dan score di jadiikan string

Medium: rigidbody pada Tapcontroller.cs tidak bisa inheritance karena penamaan; solusi nya di ganti dengan rename ke rigidBody.

High: Pada GameManager.cs +CountdownText.OnCountdownFinished += OnCountdownFinished; tidak ada pada void OnEnable() menyebabkan null references; solusi CountdownText.OnCountdownFinished += OnCountdownFinished; di tambahkan pada OnEnable()
      
   +Deadzone tag tidak di temukan pada bottom wall di prefab; solusi pasang tag di bottom wall
      
   +public bool GameOver { get { return gameOver; } } memiliki typo tanda ! pada gameOver sehingga game over page tidak muncul
   
   + Pada TapController.cs salah arah AddForce pada vector2.down sehingga menyebabkan plane turun; solusi di ganti menjadi : rigidBody.AddForce (Vector2.up * tapForce, ForceMode2D.Force);

Low: Kesalahan di GameManager.cs pada symbol di (score < savedScore) pada OnPlayerDied menybabkan tidak munculnya highscore; solusi < di ubah menjadi >
