pipeline {
    agent any 

    stages {
        stage('Checkout du Code') {
            steps {
                // Cette étape est gérée automatiquement par Jenkins grâce à la configuration SCM
                echo 'Code cloné depuis le dépôt distant via SCM.'
            }
        }
        
        stage('Archiver le Résultat') {
            steps {
                // Archive le fichier helloworld.html présent dans l'espace de travail
                archiveArtifacts artifacts: 'helloworld.html', fingerprint: true
            }
        }
    }
}
