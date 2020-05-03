# Belajar Babel Dasar

npm install @babel/core babel-loader @babel/preset-env --save-dev

module: {
        rules: [
            {
                test: /\.js$/,
                exclude: "/node_modules/",
                use: [
                    {
                        loader: "babel-loader",
                        options: {
                            presets: ["@babel/preset-env"]
                        }     
                    }
                ]
        ]   }
    }        
// contoh